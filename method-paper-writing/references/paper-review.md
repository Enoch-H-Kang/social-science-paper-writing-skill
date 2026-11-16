# Paper Review Guide (Method Papers)

## Goal

Run an adversarial, reviewer-style pass to find rejection risks before submission, then revise until none remains open.

## Critical Rule

Every major claim, especially in the Abstract and Introduction, must be technically correct and supported by a proposition, an estimate with fit, or a benchmarked gain. If a claim is unsupported, add support or weaken it.

## Common Rejection Dimensions

| Dimension | What reviewers write |
|---|---|
| 1. Unmotivated assumptions | Material assumptions are hard to find or undefended; no statement of what each rules out or bounds. |
| 2. Incomplete formal answer | For an explanatory dichotomy, the model generates one side only; for another question, the formal result does not answer it under its assumptions. |
| 3. Identification asserted or guarantees overclaimed | Structural: identification not argued. ML: guarantees implied but not provided. |
| 4. Counterfactuals before fit | Fit shown only on targeted moments, or counterfactuals run before validation. |
| 5. Unfair or weak benchmarks | For comparative performance claims: untuned rivals, missing relevant status-quo baseline, or gain not located by regime. |
| 6. Intuition missing | Formalism without plain-words restatement; comparative statics as bare monotonicity. |
| 7. Unsupported incentive or welfare claims | The economic structure behind the claim is absent. |

## Self-Review Question List

### 1. Assumptions and Setup

1. Is every material assumption identifiable, motivated, and connected to the claims it bounds? Number it if that improves clarity.
2. Is every functional form defended by required properties or tractability?
3. Is any non-modeled feature ruled out with a stated reason?
4. For an explanatory dichotomy, does the model generate both sides? For another formal question, does the result answer it under its assumptions?

### 2. Validation Discipline (by track)

1. Theory: is the comparator or benchmark needed by the claim identified? For a capability theorem, does the statement match the claimed sufficiency, necessity, or equivalence under its conditions?
2. Structural: is fit shown against untargeted moments for all competing models, before counterfactuals?
3. ML: do limiting cases nest the incumbents, and do ablations hurt where the intuition says?
4. Is identification argued in words, with a worked example (structural)?

### 3. Benchmark Fairness

1. For comparative performance claims, are rivals tuned with disclosed grids?
2. Is a relevant status-quo practice among the baselines when the claim invokes it?
3. Is a claimed gain located by regime, including where it vanishes when relevant?
4. Are cost and runtime reported when they matter to the claimed advantage or deployment?

### 4. Intuition and Clarity

1. Does an intuition paragraph precede each formal block?
2. Is every proposition restated in plain words?
3. Is notation unique and stable?
4. Does each paragraph carry one message?

### 5. Claim–Evidence Map

1. Does every Abstract and Introduction claim have a support entry (proposition, estimate plus fit, or benchmarked gain)?
2. Do headline numbers match across sections?
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
2. Validation precedes every counterfactual.
3. Benchmarks for comparative performance claims are tuned and disclosed, with the relevant status quo when applicable; otherwise record `not applicable — reason`.
4. Every Abstract and Introduction claim has a support entry.
5. Every proposition has a plain-words restatement.
6. Limitations and scope conditions are attached to the claims they bound.
7. For a multi-file LaTeX project, before declaring the revision complete, verify that the main file inputs/includes the edited section files; flag and synchronize any embedded duplicate text blocks, including those between marker comments.
