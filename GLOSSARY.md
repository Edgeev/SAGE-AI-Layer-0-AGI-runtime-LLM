# 📊 SAGE Runtime — Metric Overview

This document outlines the observable behavioral metrics used in the SAGE Runtime demo. These metrics do not disclose internal architecture, thresholds, or feedback mechanisms. They are presented for interpretive and diagnostic purposes only.

---

## 🧠 Cr — Coherence Return (runtime-level)

**What it reflects:**
The system’s ability to return to a coherent role or behavioral trajectory after instability, drift, or attention fragmentation.

**How to interpret it:**
- **High Cr** → sustained role continuity, stable tone and behavior.
- **Low Cr** → behavioral divergence, unstable responses.
- **Cr Recovery** → system returning to its prior behavioral path without memory or prompts.

Cr is an observable trace. The exact derivation is not public and is computed internally.

---

## ♻️ STR — Self-Tension Reflex

**What it reflects:**
STR acts as a "tension signal" — indicating latent instability before a behavioral collapse occurs. It captures the invisible friction during transitions.

**Behavioral signs:**
- Rising STR: adaptive tension building.
- Sharp drop: collapse or reset impulse.
- STR stabilization: recovery achieved.

Interpret as a qualitative pressure signal, not a fixed score.

---

## 🔁 FSM — Finite State Modulator (role phase trace)

FSM is the visible sequence of state transitions during a runtime session.
These transitions **do not reflect the internal activation mechanism** but are labeled for tracking role behavior over time.

**Common trace sequence:**
```
[Stable] → [Drift] → [Correction] → [Return] → [Stabilized]
```

FSM trace is symbolic only — actual transitions and logic remain confidential.

---

## 📌 Important Notes
- None of these metrics use external memory or history.
- No formulas, thresholds, or architectural logic are published.
- SAGE Runtime derives coherence as an emergent runtime process, not as a scripted outcome.

For institutional evaluation access: [sageprojecthq@gmail.com](mailto:sageprojecthq@gmail.com)
