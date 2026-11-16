# Paper Review Guide (Method Papers)

## Goal

Run an adversarial, reviewer-style pass to find rejection risks before submission, then revise until none remains open.

## Critical Rule

Every major claim, especially in the Abstract and Introduction, must be technically correct and supported by a proposition, an estimate with fit, or a benchmarked gain. If a claim is unsupported, add support or weaken it.

## Common Rejection Dimensions

| Dimension | What reviewers write |
|---|---|
| 1. Unmotivated assumptions | Functional forms and assumptions are undefended; no statement of what each rules out. |
| 2. Favorite regime only | The model generates one side of the phenomenon; no benchmark model; no dichotomy check. |
| 3. Identification asserted or guarantees overclaimed | Structural: identification not argued. ML: guarantees implied but not provided. |
| 4. Counterfactuals before fit | Fit shown only on targeted moments, or counterfactuals run before validation. |
| 5. Unfair or weak benchmarks | Untuned rivals, no status-quo baseline, gain not located by regime. |
| 6. Intuition missing | Formalism without plain-words restatement; comparative statics as bare monotonicity. |
| 7. Unsupported incentive or welfare claims | The economic structure behind the claim is absent. |

## Self-Review Question List

### 1. Assumptions and Setup

1. Is every assumption numbered, motivated, and paired with what it rules out?
2. Is every functional form defended by required properties or tractability?
3. Is any non-modeled feature ruled out with a stated reason?
4. Does the model generate both sides of the phenomenon (theory)?

### 2. Validation Discipline (by track)

1. Theory: is there a benchmark model, and is the main result stated against it?
2. Structural: is fit shown against untargeted moments for all competing models, before counterfactuals?
3. ML: do limiting cases nest the incumbents, and do ablations hurt where the intuition says?
4. Is identification argued in words, with a worked example (structural)?

### 3. Benchmark Fairness

1. Are rivals tuned with disclosed grids?
2. Is the status-quo practice among the baselines?
3. Is the gain located by regime, including where it vanishes?
4. Are cost and runtime reported?

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
3. Mark each item `pass`, `needs revision`, or `needs new analysis`.
4. Revise claims, writing, analyses, or scope accordingly.
5. Repeat until no major rejection risk remains.

## Checklist

1. No dimension 1–5 risk remains open.
2. Validation precedes every counterfactual.
3. Every benchmark is tuned, disclosed, and includes the status quo.
4. Every Abstract and Introduction claim has a support entry.
5. Every proposition has a plain-words restatement.
6. Limitations and scope conditions are attached to the claims they bound.
