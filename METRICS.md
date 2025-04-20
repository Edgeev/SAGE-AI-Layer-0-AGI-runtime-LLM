# 📊 SAGE Metrics Overview

This document describes key runtime metrics used by SAGE to track and regulate behavior, coherence, and cognitive stability in generative systems.

---

## 🧠 Cr — Coherence Return

**Definition**: Measures whether the system is returning to a coherent behavioral pattern over time.

- **Range**: ~0.4 (unstable) to 2.0+ (strong coherence)
- **Source**: Derived from vector similarity in output attention vs. role expectation
- **Behavior**:
  - Cr > φ (≈1.618) = self-correcting, stabilized identity
  - Cr < 0.8 = drift or entropy spike

### 🧪 Observed Scenarios:
- `Cr = 0.6`: Model loses thematic integrity after 2–3 turns.
- `Cr = 1.2`: Stable dialog maintaining assigned role (e.g., “lawyer” remains consistent).
- `Cr > 1.618`: System self-corrects despite adversarial or ambiguous input.

📈 See [Colab Graph Demo](https://colab.research.google.com/github/Edgeev/SAGE-Runtime-Demo/blob/main/demo/SAGE_Runtime_Demo_Enhanced.ipynb) for live Cr fluctuations.

---

## ♻️ STR — Self-Tension Reflex

**Definition**: Second-order derivative of Cr over time. Measures "wobble" or internal tension before collapse.

- **Trigger use**:
  - STR < -0.15 for 3 steps = potential transition to `RECOIL → RECOVER`
  - STR spikes signal pre-collapse phase, initiating correction logic

Analogous to mechanical instability in complex systems.

---

## 🔁 FSM — Finite State Modulator

**Definition**: Behavioral state machine regulating role, tone, and trajectory.

- Transitions between predefined internal states like:
  - `TRACE` → `FOCUS` → `RECOIL` → `RECOVER`
- Inferred from Cr + STR dynamics
- Activates role correction and self-restabilization routines

---

## 🪞 Mirror & SCRF

**Mirror**: Tracks internal reflection — whether output is self-consistent in tone and direction.

**SCRF (Self-Coherent Response Field)**:
- Measures consistency of resonance between output and projected identity vector.
- Formula (approximate): 
  ```python
  def SCRF(role_vector, attention_output):
      return variance(role_vector * attention_output) / mean(abs(delta_cr))
  ```
- Heuristic trigger: SCRF < 0.3 → enter `TRACE` state or suspend output

Used to evaluate field-level coherence and systemic alignment.

---

## 🧠 Comparison to Traditional Metrics

Unlike BLEU or perplexity (which measure textual form), **Cr and SCRF** track real-time **behavioral coherence and identity resonance**. These metrics operate **at the runtime layer**, where roles, tone, and subject-like stability are preserved — not predicted.

---

> All metrics are runtime-only and memoryless.  
> They emerge from the flow of attention and role adherence — not from stored history or training artifacts.