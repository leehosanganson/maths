# Real Analysis — A Rigorous Syllabus

## Philosophy

This syllabus is designed for someone with an **engineering + data science background** who wants to **re-learn mathematics rigorously**. You've already taken calculus and linear analysis; the goal here is not to learn new computation techniques, but to build the kind of deep understanding that makes proofs feel natural.

The pace targets approximately **5–8 hours per week**, structured as **2-week sprints**: Week 1 for self-study (reading + notes), Week 2 for problem sets (proofs + exercises). This is not a race — it is a deliberate re-building of mathematical maturity.

## How to Use This Syllabus

Each sprint covers a two-week period:

- **Week 1:** Self-study the topics listed in the "Topics" section. Read the recommended primary text, watch supplementary lectures if helpful, and take organized notes.
- **Week 2:** Work through the problem set. These are proof-heavy exercises drawn from the recommended texts. The goal is to write clean proofs, not just find answers.

Use the GitHub Issue templates (`notes.md` and `pset.md`) to track progress for each sprint. Create one issue per sprint with two sub-issues (or a combined tracker) following the template structure.

## Sprints

---

### Sprint 1: The Real Number System & Archimedean Property

**Week 1 — Topics:**
- Ordered fields and the ordered field axioms
- The supremum (least upper bound) property and its equivalence to completeness
- Density of $\mathbb{Q}$ between any two distinct reals
- Brief overview of constructions: how $\mathbb{R}$ arises as a completion of $\mathbb{Q}$

**Week 2 — Problem Set Focus:**
- Prove density of $\mathbb{Q}$ in $\mathbb{R}$ (for any $a < b$, find $q \in \mathbb{Q}$ with $a < q < b$)
- Prove every non-empty set bounded below has an infimum
- Work through basic epsilon-N arguments for limits of sequences

**Recommended Resources:**
- *Understanding Analysis* (Abbott), Chapter 1
- *Principles of Mathematical Analysis* (Rudin), Chapter 1
- Tao's lecture on real numbers (YouTube)

**Dependencies:** None — this is the foundation.

---

### Sprint 2: Sequences & Convergence

**Week 1 — Topics:**
- Limits of sequences and the formal epsilon-N definition
- Uniqueness of limits
- Subsequences and their relationship to convergence
- Boundedness of convergent sequences
- Monotone Convergence Theorem
- Cauchy sequences; completeness revisited

**Week 2 — Problem Set Focus:**
- Prove every convergent sequence is bounded
- Prove that every monotone bounded sequence converges (Monotone Convergence Theorem)
- Prove the Cauchy criterion for convergence
- Work through epsilon-N proofs for specific sequences

**Recommended Resources:**
- *Understanding Analysis* (Abbott), Chapter 2
- *Principles of Mathematical Analysis* (Rudin), Sections 3.1–3.4
- Tao's lectures on sequences

**Dependencies:** Sprint 1 — comfort with epsilon-delta arguments.

---

### Sprint 3: Series & Bolzano-Weierstrass

**Week 1 — Topics:**
- Infinite series: partial sums, convergence definitions
- Absolute vs. conditional convergence
- Comparison tests, ratio test, root test
- Bolzano-Weierstrass theorem (every bounded sequence has a convergent subsequence)
- Introductory thoughts on compactness

**Week 2 — Problem Set Focus:**
- Prove the Alternating Series Test
- Apply Bolzano-Weierstrass to find convergent subsequences in given sequences
- Prove that every bounded infinite subset of $\mathbb{R}$ has a limit point

**Recommended Resources:**
- *Understanding Analysis* (Abbott), Chapter 3
- *Principles of Mathematical Analysis* (Rudin), Section 3.5
- Tuckerman's lectures on series

**Dependencies:** Sprint 2 — sequence convergence and boundedness.

---

### Sprint 4: Functions & Continuity

**Week 1 — Topics:**
- Epsilon-delta definition of limits for functions
- Limits of functions vs. limits of sequences
- Topological view of continuity (open and closed sets)
- Intermediate Value Theorem (IVT)
- Extreme Value Theorem (EVT)

**Week 2 — Problem Set Focus:**
- Prove the Intermediate Value Theorem
- Prove the Extreme Value Theorem
- Work through direct proofs of continuity for specific functions
- Prove that the composition of continuous functions is continuous

**Recommended Resources:**
- *Understanding Analysis* (Abbott), Chapter 4
- *Principles of Mathematical Analysis* (Rudin), Sections 2.1–2.6

**Dependencies:** Sprint 3 — compactness intuition; Sprint 2 — sequence limits.

---

### Sprint 5: Differentiation

**Week 1 — Topics:**
- Mean Value Theorem (MVT) and its proof
- L'Hôpital's Rule (derivations and limitations)
- Taylor's Theorem (with remainder forms)
- Derivatives and injectivity (monotonicity)
- Pathological counterexamples: functions that are continuous but not differentiable

**Week 2 — Problem Set Focus:**
- Prove the Mean Value Theorem
- Apply Taylor's Theorem to estimate function values
- Prove that differentiability implies continuity
- Work through derivative counterexamples (e.g., Weierstrass function intuition)

**Recommended Resources:**
- *Understanding Analysis* (Abbott), Chapter 5
- *Principles of Mathematical Analysis* (Rudin), Chapter 5
- Supplementary counterexample collections (see resources below)

**Dependencies:** Sprint 4 — continuity, compactness.

---

### Sprint 6: Uniform Convergence & Power Series

**Week 1 — Topics:**
- Pointwise vs. uniform convergence (definitions and examples)
- Continuity of limit functions under uniform convergence
- Power series: radius of convergence, term-by-term operations
- Definitions of $e^x$, $\sin x$, $\cos x$ via power series

**Week 2 — Problem Set Focus:**
- Prove that uniform convergence preserves continuity
- Prove the Weierstrass M-test
- Work through uniform convergence proofs for specific function sequences (e.g., $x^n/n$, $\sin(nx)/n$)

**Recommended Resources:**
- *Understanding Analysis* (Abbott), Chapter 6
- *Principles of Mathematical Analysis* (Rudin), Chapter 7
- Supplementary video lectures on uniform convergence

**Dependencies:** Sprint 5 — Taylor series intuition; Sprint 4 — continuity.

---

### Sprint 7: Integration (Riemann)

**Week 1 — Topics:**
- Riemann sums and the definition of the Riemann integral
- Integrability conditions: upper and lower sums, Darboux approach
- Fundamental Theorem of Calculus (both parts)
- Improper integrals and convergence tests

**Week 2 — Problem Set Focus:**
- Prove the Fundamental Theorem of Calculus
- Prove that every continuous function on a closed interval is Riemann integrable
- Work through constructing examples of non-integrable functions (e.g., Dirichlet function)

**Recommended Resources:**
- *Principles of Mathematical Analysis* (Rudin), Chapter 6
- Abbott's treatment of integration (Chapter 7 if you use his book)
- Tuckerman's lectures on integration

**Dependencies:** Sprint 4 — continuity; Sprint 5 — derivatives.

---

### Sprint 8: Metric Spaces & General Topology *(Extension)*

**Week 1 — Topics:**
- Metric spaces: definition and examples
- Open and closed sets in arbitrary metric spaces
- Compactness generalized (Heine-Borel theorem extension)
- Completeness in general metric spaces
- Dense subsets and separability

**Week 2 — Problem Set Focus:**
- Prove the Banach Fixed Point Theorem
- Work through topology exercises in general metric spaces
- Prove completeness of specific function spaces (e.g., $C[a,b]$ with sup norm)

**Recommended Resources:**
- *General Topology* (Munkres), Chapter 2
- Rudin, Chapter 2 (generalized treatment)
- Supplementary lecture notes on metric spaces

**Dependencies:** Sprint 7 — completeness intuition; all prior sprints for proof maturity.

---

### Sprint 9: Enrichment / Lebesgue Preview

**Week 1 — Topics:**
- Measure-zero sets and their properties
- Comparison of Riemann vs. Lebesgue integration (conceptual)
- Optional: distributions (intro to functional analysis perspective)

**Week 2 — Problem Set Focus:**
- Prove the Cantor set has measure zero
- Conceptual exercises bridging forward to measure theory
- Reflect on what was gained from the rigorous approach

**Recommended Resources:**
- Tao's *Analysis I*, Chapter 11+
- Rudin, Chapter 11 (optional)
- YouTube lectures on measure theory / Lebesgue integration

**Dependencies:** All prior sprints — this sprint is enriching and forward-looking.

---

## Recommended Primary Texts (Summary)

| Text | Focus | Best For |
|------|-------|----------|
| Abbott, *Understanding Analysis* | Intuitive entry point with proofs | Weeks 1–6 |
| Rudin, *Principles of Mathematical Analysis* | Concise, theorem-proof style | Sprint reviews, reference |
| Tao, *Analysis I* | Detailed, pedagogical approach | Supplementary reading |

## Supplementary Resources

- **Tuckerman's lectures** (YouTube) — excellent for series and integration
- **Tao's lecture series** — great for foundational concepts
- **Counterexample collections** — see [MathOverflow](https://mathoverflow.net) or specific university notes for pathological functions
- **Munkres, *Topology*** — for Sprint 8 and onward
- **YouTube channels:** 3Blue1Analysis (intuition), Dr. Trefz Baz (proofs)

## Progress Tracker

| Sprint | Status | Week 1 Done | Week 2 Done | Notes |
|--------|--------|-------------|-------------|-------|
| 1 | — | — | — | |
| 2 | — | — | — | |
| 3 | — | — | — | |
| 4 | — | — | — | |
| 5 | — | — | — | |
| 6 | — | — | — | |
| 7 | — | — | — | |
| 8 | — | — | — | |
| 9 | — | — | — | |
