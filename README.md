<h1 align="center">Michael Forsythe Robinson</h1>
<p align="center">
  <strong>Applied Generative AI · Agentic Systems · Research Engineering</strong>
</p>
<p align="center">
  <em>Building AI systems that distinguish between an answer, an inference, and the evidence for an answer.</em>
</p>

<p align="center">
  <a href="https://orcid.org/0009-0002-8487-759X"><img src="https://img.shields.io/badge/ORCID-0009--0002--8487--759X-a6ce39?style=flat-square&logo=orcid"></a>
  <a href="https://www.linkedin.com/in/michael-forsythe-robinson-082255391"><img src="https://img.shields.io/badge/LinkedIn-Michael%20Forsythe%20Robinson-0A66C2?style=flat-square&logo=linkedin"></a>
  <a href="https://portfolio-hub-kappa-murex.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-Command%20Center-007ACC?style=flat-square&logo=vercel"></a>
  <a href="https://substack.com/@mforsytherobinson"><img src="https://img.shields.io/badge/Substack-Research%20Publications-FF6719?style=flat-square&logo=substack"></a>
  <a href="https://www.amazon.com/author/mforsytherobinson"><img src="https://img.shields.io/badge/Amazon-Author%20Catalog-232F3E?style=flat-square&logo=amazon"></a>
</p>

---

### Abstract

I'm an independent AI systems architect, research engineer, and technical author working at the intersection of generative AI, agentic systems, causal inference, and formal reasoning. My work treats evidence, uncertainty, provenance, and falsifiability as engineering primitives rather than afterthoughts.

The organizing question behind my 2026 research: **can an AI system distinguish between an answer, an inference, and the evidence for an answer** — and keep those states from silently collapsing into each other?

<!-- Optional hero image — keep if it's your own diagram/photo, drop if it reads as decorative for this audience -->
<!-- <img width="1376" height="768" alt="The_Causal_Architect_-_Slide_1" src="https://github.com/user-attachments/assets/1856e964-79f4-4006-92df-d73083020d05" />
 -->

---

### I. Research Architecture

The pipeline below maps how a piece of source knowledge moves through my systems, from raw text to something you could act on.

```text
KNOWLEDGE
   │
   ▼
LATENT DISCOVERY        (LIDE — cross-source relationship discovery)
   │
   ▼
STRUCTURAL EXTRACTION    (Cangjie-Deconstructor — text → typed primitives)
   │
   ▼
FORMALIZATION            (Cognitive Compiler — primitives → executable spec)
   │
   ▼
EVIDENCE-GOVERNED EVAL.   (IEF — claim → proposition → evidence → status)
   │
   ▼
VERIFICATION              (Three-Gate Protocol — blind review, mutation testing)
   │
   ▼
CAUSAL / DECISION SYSTEMS
   │
   ▼
KNOWLEDGE TRANSFER        (curriculum, writing, teaching)
```

---

### II. A Failure, Documented

> "A system should be able to reduce confidence when the evidence gets worse."

An early pass at a large SUNDS (Sudden Unexpected Death Syndrome) dataset appeared to show an association between geomagnetic activity and mortality. The signal was compelling. Rebuilding the pipeline from scratch showed it was a data-processing artifact, not a real effect.

The result that mattered wasn't the original finding — it was the correction. That's the design principle behind the evidence-governed architecture below: don't protect the hypothesis, protect the calibration.

*[Note: link the writeup or dataset here if you have one you can share publicly — right now this is the strongest anecdote in the document and the only one without a citation.]*

| Paradigm | Inferential Flow | Terminal State |
|---|---|---|
| Traditional | Claim → Evidence → Insufficient Data → *"Probably True"* | Overconfidence |
| Evidence-Governed | Claim → Evidence → Evaluation → Contradiction / Gap | `UNKNOWN` / `REJECTED` / `QUALIFIED` |

The goal isn't pessimism. It's calibration.

---

### III. Core Research Systems

**1. Invention Evaluation Framework (IEF)**
An evidence-governed, multi-agent system for evaluating inventions and technical claims against patents and literature, with every conclusion traced to a source.
- Pipeline: `CLAIM → PROPOSITION → EVIDENCE → SOURCE → INFERENCE → EPISTEMIC STATUS`
- Validation: multi-lane DAG review, blind re-verification, mutation testing, acceptance contracts
- Goal: make AI-assisted evaluation auditable, not just plausible-sounding

**2. Latent Information Discovery Engine (LIDE)**
Instead of "what's similar to my query," asks "what relationships exist in this corpus that nobody explicitly looked for" — reciprocal-rank fusion, graph traversal, equation fingerprinting, cross-domain analogy detection, with an explicit falsification stage.

**3. Cognitive Compiler & Cangjie-Deconstructor**
Cangjie decomposes source text into typed primitives, operators, and constraints; the Cognitive Compiler turns those into typed intermediate representations for downstream reasoning. `Literature → Structure → Mechanism → Model.`

**4. Leonardo Lab**
Extends the compiler into architecture search — extracting design constraints from existing systems (e.g. transformer attention variants) and exploring the implied design space.

**5. Three-Gate Research Protocol**
An operating procedure for keeping discovery from quietly turning into belief: `DISCOVER → GENERATE → GATE → VERIFY → CHASE DROPPED THREADS → GRADE → WRITE.` A failed hypothesis is a result, not wasted effort.

---

### IV. Causal Inference & Production Systems

Before the current research direction, I built production marketing-science and causal-inference systems — still the quantitative foundation of the work above.

| System | Description | Benchmark *(self-reported — link source if available)* |
|---|---|---|
| Streaming attribution engine | Real-time Markov-Shapley attribution over stateful stream processing | ~200K events/sec, sub-100ms p99 |
| Probabilistic identity resolution | Privacy-conscious cross-device matching | ~78–98% match rate range, verify exact figure |
| Causal experimentation framework | Synthetic control, DiD, placebo testing, bootstrap inference | — |
| Experimentation platform | CUPED, sequential testing, O'Brien-Fleming boundaries | ~30–35% variance reduction |

**Methods:** structural causal models, difference-in-differences, synthetic control, double ML, Bayesian hierarchical priors (NUTS/HMC), adstock/saturation modeling.

*I've left the benchmark numbers roughly as given but flagged them — for a professional-audience document, each of these should link to the dashboard, repo, or writeup that produced it, or drop the number and keep the method description.*

---

### V. Applied Generative AI & Agentic Systems

`Prompt → Structured Extraction → Tool Use → Agent Orchestration → Data/API Integration → Evaluation → Observability → Production`

- **FrontDesk.ai** — an agentic AI voice-receptionist platform, used as a live testbed for agent design, structured outputs, and production evaluation under real usage rather than demo conditions.

---

### VI. Curriculum

*AI Builder's Launchpad* — a five-volume series on the applied-AI lifecycle:

1. From First Prompts to First Modular Pipeline
2. Automating the Intelligence: Python, APIs, and Data for AI Pipelines
3. Building a Digital Brain: Production AI System Architecture
4. Moving to Production: Deployment, Monitoring, Security, Management
5. A Strategist's Guide to AI: Building an AI-Native Business

Philosophy: don't just teach what AI is — teach how to build it.

---

### VII. Research Philosophy

1. **Evidence before certainty.** A compelling explanation isn't automatically a supported one.
2. **Mechanisms over labels.** Why things connect matters more than that they correlate.
3. **Reproducibility is infrastructure.** Results should be recoverable from versioned artifacts, not just claimed.
4. **Uncertainty has to survive the pipeline.** `Unknown ≠ Probably True ≠ Supported ≠ Established` — these shouldn't collapse into each other.
5. **A negative result is still a result.** Failures expose broken measurements and better questions.

> `Build → Measure → Break → Audit → Repair → Test → Document → Ship`
> A system that survives a deliberate attempt to break it is more interesting than one that just gives a good demo.

---

### VIII. Beyond the Pipeline

Systems are abstractions; their consequences aren't. Time spent with rescued wildlife shaped how I think about that gap — the same discipline that preserves provenance in a data pipeline should ultimately serve something outside it.

That's the starting point for **Surveillance Humanism** — work exploring the line between behavioral intelligence and humanitarian intervention. Where surveillance capitalism asks how to monetize what people disclose to machines, this asks how the same signal could reduce harm — crisis intervention, epidemiological signaling, protecting vulnerable populations — treating privacy and false-positive risk as design constraints from the start, not an afterthought.

---

### IX. Output — *(verify every number below before publishing)*

| Category | Claimed | Status |
|---|---|---|
| Curriculum volumes | 5 | ✅ listed above, verifiable by content |
| Technical whitepapers | 10 | ⚠️ link each one |
| Research programs | 11+ | ⚠️ define what counts as a "program" |
| Research papers/artifacts | ~80 | ⚠️ needs a source list or drop the number |
| Causal intelligence modules | 9 | ⚠️ link each |
| Production AI systems | 30+ | ⚠️ "production" implies live/deployed — confirm which ones actually are |
| Published DOIs | 10+ | 🚩 at least one badge checked resolves to a placeholder DOI (`zenodo.12345678`) — audit all before claiming this number |

I left this as a table instead of prose on purpose — it's the part of the document most likely to get fact-checked, and right now it's the least defensible part of an otherwise strong pitch.

---

### X. Open Research Artifacts

- 🧠 [**First-Principles Attribution**](https://github.com/Michaelrobins938/first-principles-attribution) — Markov chains + Shapley values + Bayesian UQ for the correlation/causation gap.
- 🌪️ [**The Same Storm in Two Machines**](https://github.com/Michaelrobins938/The-Same-Storm-in-Two-Machines-Plasma-storm-unification) — cross-community synthesis on MHD-generator streamers vs. Hall-thruster rotating spokes.
- 🌐 [**Plasma-Assisted Boundary Dynamics**](https://github.com/Michaelrobins938/Plasma-Assisted-Boundary-Dynamics-and-Material-Memory-in-Extreme-Weather) — state-space framework for history-dependent extreme-weather damage inference.
- 🚀 [**Portfolio-Hub**](https://github.com/Michaelrobins938/portfolio-hub) — command-center portfolio of attribution and data-science projects.

*(Dropped FEP from this list — as of the last audit it's protocol documents with no executable code, which undercuts the "evidence-governed, auditable" framing this section is making. It's a legitimate research protocol; it just belongs in a "Research Protocols" section, not next to repos with real pipelines and tests.)*

---

### XI. Trajectory

- **2025 — Construction.** Build → deploy → measure. Ideas become useful when they survive implementation.
- **2026 — Epistemics.** Discover → formalize → evaluate → verify → explain → operationalize. Implementations become trustworthy when they survive verification.

The next goal isn't more agents — it's better epistemic infrastructure under the agents already built: systems that show their work, expose their uncertainty, and get more useful the more you try to break them.

---

### XII. Connect

Open to applied research collaboration, architecture advising, and curriculum development.

<p align="center">
  <a href="mailto:michael.robins938@gmail.com"><img src="https://img.shields.io/badge/Email-Michael%20Robinson-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://portfolio-hub-kappa-murex.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-Command%20Center-000000?style=for-the-badge&logo=vercel"></a>
  <a href="https://github.com/Michaelrobins938"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white"></a>
</p>
