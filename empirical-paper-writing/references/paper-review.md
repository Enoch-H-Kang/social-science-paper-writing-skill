# Paper Review Guide (Empirical Papers)

## Goal

Run an adversarial, reviewer-style pass to find rejection risks before submission, then revise until none is open. Assume reviewers will probe every weak point.

## Critical Rule

Every major claim, especially in the Abstract and Introduction, must be technically correct and explicitly supported by an identified estimate or a held-out evaluation. If a claim is unsupported, add evidence or weaken the claim.

## Common Rejection Dimensions

| Dimension | What reviewers write |
|---|---|
| 1. Weak identification | Selection is unaddressed; the variation is not exogenous; the direction of bias is not stated. |
| 2. Mechanism not discriminated | Only mediator correlations; the strongest rival story is untested. |
| 3. Policy value in-sample or baseline-free | No off-policy or holdout evaluation; no status-quo or best-uniform comparison. |
| 4. External validity | One firm or category; no scope conditions. |
| 5. Overclaiming | Abstract numbers cannot be traced to an identified estimate. |
| 6. Incremental substance | The answer is already known, or no actor would change behavior. |

## Self-Review Question List

Answer each with explicit evidence from the paper.

### 1. Identification

1. What is the source of variation, and where in the text is it defended?
2. Which selection threat is the most dangerous, and which way does it bias the headline?
3. Are filtering, trimming, and sample-construction rules stated in the open?
4. Were splits and estimands declared before any result?

### 2. Mechanism

1. Does the scorecard rule something out, not only support something?
2. Is the strongest rival story rebutted explicitly?
3. Are non-causal links marked as such?
4. Do mechanism results match the direction of the average effect?

### 3. Results Ordering and Baselines

1. Are findings in the fixed order, independent of analysis chronology?
2. Does every gain name a baseline in the same sentence?
3. Are train and test shown side by side, with the test authoritative?
4. Are modest gains owned with a mechanical explanation?

### 4. Policy Evaluation

1. Is policy value estimated out of sample or with a bias-corrected estimator?
2. Is it compared with the status quo and the best uniform policy, with a test of the gap?
3. Are failing rival methods reported and diagnosed?
4. Are long-run consequences addressed where data exist?
5. Are scope conditions for transfer stated operationally?

### 5. Writing

1. Does each paragraph carry one message, stated first?
2. Is every claim in the Abstract and Introduction in the claim map with support and baseline?
3. Are headline numbers identical across sections?
4. Is any sentence long enough to need a second parse?

## Adversarial Workflow

1. Read the paper as a skeptical reviewer for the target journal.
2. Answer every question above with evidence from the paper.
3. Mark each item `pass`, `needs revision`, or `needs new analysis`.
4. Revise claims, writing, analyses, or scope accordingly.
5. Repeat until no major rejection risk remains.

## Checklist

1. No dimension 1–3 risk remains open.
2. Every Abstract and Introduction claim has a support entry in the claim map.
3. Every gain names its baseline and its evaluation sample.
4. Scope conditions and limitations appear in the text, attached to the claims they bound.
5. Headline numbers match across all sections.
6. Every item marked `needs new analysis` is either done or the claim it supports is weakened.
