# Paper Review Guide (Method Papers)

## Goal

Run an adversarial, reviewer-style pass to find rejection risks before submission, then revise until none remains open.

## Critical Rule

Every major claim, especially in the Abstract and Introduction, needs support appropriate to its stated strength: an analytical proof, estimate and model check, benchmark, sourced institutional fact, documented case, explicitly suggestive descriptive, or implementation argument. If a claim exceeds that support, add evidence or narrow it.

## Common Rejection Dimensions

| Dimension | What reviewers write |
|---|---|
| 1. Unmotivated assumptions | Material assumptions are hard to find or undefended; no statement of what each rules out or bounds. |
| 2. Incomplete formal answer | For an explanatory dichotomy, the model generates one side only; for another question, the formal result does not answer it under its assumptions. |
| 3. Identification asserted or guarantees overclaimed | Structural: identification not argued. ML: guarantees implied but not provided. |
| 4. Counterfactuals without model checks | Body counterfactuals rely on unchecked fit, or fitted-sample checks are described as independent held-out evidence. Truthful introductory previews are allowed. |
| 5. Unfair or weak benchmarks | For comparative performance claims: untuned rivals, missing relevant status-quo baseline, or gain not located by regime. |
| 6. Intuition missing | Formalism without plain-words restatement; comparative statics as bare monotonicity. |
| 7. Unsupported incentive or welfare claims | The economic structure behind the claim is absent. |

## Self-Review Question List

### 1. Assumptions and Setup

1. Is every material assumption identifiable, motivated, and connected to the claims it bounds?
2. Are consequential functional forms defended by required properties, institutional fit, or tractability?
3. Is any non-modeled feature ruled out with a stated reason?
4. For an explanatory dichotomy, does the model generate both sides? For another formal question, does the result answer it under its assumptions?

### 2. Validation Discipline (by track)

1. Theory: is the comparator or benchmark needed by the claim identified? For a capability theorem, does the statement match the claimed sufficiency, necessity, or equivalence under its conditions?
2. Structural: are fitted-sample model checks described accurately, and are stronger held-out or untargeted claims backed by such evidence? Do relevant checks precede body counterfactuals?
3. ML: do claimed limiting cases and ablation effects match the tested results, including reversals?
4. Is identification argued in words, with a worked example (structural)?

### 3. Benchmark Fairness

1. For comparative performance claims affected by tuning, is the rival protocol fair and disclosed?
2. Is a relevant status-quo practice among the baselines when the claim invokes it?
3. Is a claimed gain located by regime, including where it vanishes when relevant?
4. Are cost and runtime reported when they matter to the claimed advantage or deployment?

### 4. Intuition and Clarity

1. Is plain-language interpretation near each important formal block, whether before or after it?
2. Is every proposition restated in plain words?
3. Is notation unique and stable?
4. Does each paragraph carry one message?

### 5. Claim–Evidence Map

1. Can each major Abstract and Introduction claim be mapped to appropriate support, including facts, cases, proofs, suggestive descriptives, and implementation arguments?
2. Do headline numbers agree in substance across sections, allowing compatible rounding?
3. Is every incentive or welfare claim backed by explicit economic structure?
4. Are anomalies surfaced and resolved?

## Adversarial Workflow

1. Read the paper as a skeptical reviewer for the target journal.
2. Answer every question above with evidence from the paper.
3. Mark each item `pass`, `needs revision`, `needs new analysis`, or `not applicable — reason`.
4. Revise claims, writing, analyses, or scope accordingly.
5. Repeat until no major rejection risk remains.

## Checklist

1. No dimension 1–5 risk remains open.
2. Relevant model checks precede body counterfactuals built on them; introductory previews remain truthful.
3. Benchmarks for comparative performance claims use fair disclosed tuning when tuning affects the claim, with the relevant status quo when applicable; otherwise record `not applicable — reason`.
4. Every major Abstract and Introduction claim has an appropriate support entry in the reviewer’s map.
5. Every proposition has a plain-words restatement.
6. Decisive conditions are attached to the claims they bound; broader limitations may be gathered later.
7. Flag every sentence a non-specialist must reread, parse through nested clauses, or look up a word to understand; check first-use definitions without dropping terms of art, numbers, or qualifications.
8. Every citation in the draft is verified to exist and supports its exact claim; every `[CITATION NEEDED: <the claim>]` placeholder is resolved or reported to the user.
9. For a multi-file LaTeX project, before declaring the revision complete, verify that the main file inputs/includes the edited section files; flag and synchronize any embedded duplicate text blocks, including those between marker comments.
10. Are conditions stated once, in prose at the objects they constrain? Flag upfront lists, duplicated statements, and formal numbered assumption environments without a needed cross-section handle.
11. Is the main text self-contained? Flag any body passage that raises a substantive point and sends its examination, explanation, or specification to an appendix.
