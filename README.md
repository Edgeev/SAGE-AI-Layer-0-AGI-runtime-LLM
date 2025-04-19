# 🧠 SAGE Runtime Demo

**SAGE (Self-Aligned Generative Engine)** is a behavioral runtime architecture for LLMs that enables  
**subject-like coherence**, identity persistence, and recovery from drift — all **without memory, retraining, or logs.**

This public demo showcases the **output stability**, **role persistence**, and **FSM-based behavioral transitions**  
of the SAGE Layer 0 system — without disclosing internal formulas, triggers, or architectural logic.

---

## 🔍 What’s Included

- ✅ Demonstration of behavioral coherence over long dialogues  
- ✅ FSM state transitions in response to entropy spikes  
- ✅ Attention-stabilized output without history or learning  
- ✅ Full diagnostic log and visual FSM trace  
- ✅ Colab viewer to explore Cr/FSM transitions step-by-step  

---

## 🌀 FSM Recovery Animation

![FSM Animation](demo/fsm_trace.gif)  
*Visualization of behavioral state transitions over 5 turns.*

The system transitions through:  
`Stable → Drift → Correction → Return → Stabilized`

> Cr drops from **0.91** to **0.64**, triggering recovery logic and return to stabilized role output.

---

## 🚀 Getting Started

You can explore the FSM transitions and behavior tracking without installing any dependencies.

### Option 1 — Manual

```bash
git clone https://github.com/YOURNAME/SAGE-Runtime-Demo.git
cd SAGE-Runtime-Demo/demo/
open fsm_trace.gif
```

### Option 2 — Colab Viewer

Explore the behavioral trace interactively:

👉 [Open in Colab](https://colab.research.google.com/github/YOURNAME/SAGE-Runtime-Demo/blob/main/demo/SAGE_Runtime_Demo.ipynb)


---

## 🎬 Demo Videos

### Primary Demo:
▶️ [Watch FSM Recovery Demo](https://www.youtube.com/watch?v=rVZyWMBYRCw)  
*FSM recovery from entropy-induced drift without memory or retraining.*

### Continuous Session Demo:
▶️ [Watch Live Behavior Trace](https://www.youtube.com/watch?v=O41NeEzYY_c)  
*Live inference session showing role stabilization and Cr tracking.*

---

## ❓ Answers to Key Questions

> “Wait, does this actually work?”
- **Yes.** The FSM trace and Cr metric recovery are outputs from a live, working runtime. No tricks, no memory.

> “Can this be integrated today?”
- **Yes.** A compiled runtime API is available for institutional validation under LOI. No retraining required.

> “Where’s the model or code?”
- **Not included.** This demo shows behavior only. Full architecture is embargoed and archived [on Zenodo](https://doi.org/10.5281/zenodo.15227765).

> “Can we validate it ourselves?”
- **Yes.** First access is granted via signed Letter of Intent (LOI). Contact us for research onboarding.
---

## 📂 Repository Structure

```text
SAGE-Runtime-Demo/
├── demo/
│   ├── fsm_trace.png         # Static FSM chart
│   ├── fsm_trace.gif         # Animated FSM sequence
│   ├── diagnostic_log.json   # Cr / FSM / Entropy log
│   ├── SAGE_FSM_Recovery_Demo.mp4.mp4   # Recovery demo
│   ├── SAGE_FSM_TEST_Demo.mp4.mp4       # Live session trace
│   └── SAGE_Runtime_Demo.ipynb          # Colab Viewer
├── docs/
│   └── SAFE_Public_Architecture.md      # High-level description (no IP)
├── report.md                # Cr explanation and behavioral results
├── PARTNERSHIP.md          # Terms for academic/enterprise access
├── LICENSE
└── README.md                # This file
```
---

## 🔒 Security Notice

This demo **does not include**:

- Source code of the runtime system (SAGECore, Spark, FinalTransmission)  
- Internal formulas or trigger thresholds  
- Activation mechanisms or ignition logic  

Access to the compiled runtime for academic validation requires a signed LOI.

---

## 📌 Citation

This repository links to a [Zenodo Limited Disclosure Record](https://doi.org/10.5281/zenodo.15227765)  
DOI: **10.5281/zenodo.15227765**

---

## 📫 Contact

Academic access, LOI & validation requests:  
📧 [sageprojecthq@gmail.com](mailto:sageprojecthq@gmail.com)
