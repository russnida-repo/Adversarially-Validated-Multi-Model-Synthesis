AVMS is a structured methodology for producing robust, defensible conclusions from multiple AI systems by explicitly separating **generation**, **interpretation**, **adversarial testing**, and **corrective integration**.

Rather than treating agreement as correctness, AVMS treats agreement as a *hypothesis to be tested*.

---

## Full Specification

The complete AVMS specification is available in the following formats:

- 📘 **Markdown (recommended for browsing):**  
  [`docs/AVMS.md`](AVMS.md)

- 📄 **PDF (formatted version):**  
  [`docs/AVMS.pdf`](AVMS.pdf)

These documents contain the full formal description of the AVMS methodology, including all phases, divergence handling, adversarial validation logic, and MP-AVMS extensions.

---

## Core Idea

Most ensemble or multi-model workflows assume that convergence implies truth.  
AVMS rejects this assumption.

Instead, it treats:
- **agreement and disagreement as diagnostic signals**
- **divergence as information, not noise**
- **adversarial challenge as a required validation step**

The result is a reasoning process that prioritizes *error detection, robustness, and epistemic resilience* over superficial consensus.

---

## The Four Phases of AVMS

### Phase 1 — Independent Generation (Divergence)
Models independently analyze the same problem without exposure to each other.

Purpose:
- Maximize epistemic diversity
- Surface alternative framings
- Prevent premature convergence

Agreement at this stage is **not validation** — it is a signal requiring interpretation.

---

### Phase 2 — Pattern Interpretation (Convergence & Divergence)
Outputs are analyzed to classify:
- convergence
- structured divergence
- chaotic divergence
- implicit assumptions

Both agreement and disagreement are treated as meaningful signals.

This phase determines whether to:
- proceed normally,
- escalate scrutiny,
- reframe the question,
- or branch into MP-AVMS.

---

### Phase 3 — Adversarial Validation
Provisional conclusions are stress-tested using adversarial challenges.

Typical challenges include:
- hidden assumptions
- alternative causal models
- competing stakeholder views
- structural failure modes
- boundary-condition violations

Weak or repetitive critiques are discarded. Strong competing explanations are retained.

---

### Phase 4 — Corrective Integration
Validated critiques are integrated into a refined synthesis by:
- bounding claims
- separating mechanisms
- qualifying uncertainty
- discarding unsupported assumptions

The output is a conclusion that has *survived structured attack*, not mere consensus.

---

## Multi-Perspective AVMS (MP-AVMS)

Some domains involve fundamentally incompatible optimization criteria (e.g., policy vs budget vs engineering).

MP-AVMS extends AVMS by:
1. Running a full AVMS cycle **per perspective**
2. Treating each result as an independent artifact
3. Performing a meta-level AVMS across perspectives

This prevents:
- premature integration
- false equivalence
- collapsing incompatible constraints

---

## Relationship to ARMOR

AVMS defines *process*.
ARMOR defines *evaluation lenses*.

Typical mapping:
- AVMS Phases 1–2 → claim generation
- AVMS Phase 3 → ARMOR-guided stress testing
- AVMS Phase 4 → filtered integration

Together they form a complete epistemic validation stack.

---

## When to Use AVMS

Recommended for:
- high-stakes reasoning
- governance and policy analysis
- safety and risk evaluation
- adversarial or ambiguous domains
- multi-stakeholder decision problems

Not recommended for:
- simple factual lookups
- low-risk creative work
- time-critical decisions
- exploratory brainstorming

---

## Status

This repository documents a *methodological framework*, not an algorithm.
It is designed for human–AI workflows, governance processes, and evaluation systems.

Contributions, critiques, and extensions are welcome.

---

## License

© 2025 Russell Nida  
Licensed under **Creative Commons Attribution–NonCommercial–ShareAlike 4.0 (CC BY-NC-SA 4.0)**.

See [`LICENSE.md`](LICENSE.md) for full terms.


