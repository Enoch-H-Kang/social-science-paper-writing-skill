# Paper Review Guide (Empirical Papers)

## Goal

Run an adversarial, reviewer-style pass to find rejection risks before submission, then revise until none is open. Assume reviewers will probe every weak point.

## Critical Rule

Every major claim, especially in the Abstract and Introduction, needs support appropriate to its stated strength: an identified estimate, independent policy evaluation, sourced institutional fact, documented case, analytical proof, explicitly suggestive descriptive, or implementation argument. If support is weaker than the wording, add evidence or narrow the claim.

## Common Rejection Dimensions

| Dimension | What reviewers write |
|---|---|
| 1. Weak identification | Selection or the source of variation is unaddressed; a stated bias sign lacks support. |
| 2. Mechanism overclaimed | Suggestive mediator links are called identified effects, or tested rivals and opposing channels are misrepresented. |
| 3. Learned-policy value unsupported | An independent or suitable off-policy evaluation and relevant comparator are missing for the gain claimed. |
| 4. External validity | One firm or category; no scope conditions. |
| 5. Overclaiming | Abstract claims exceed the support appropriate to their type or stated strength. |
| 6. Incremental substance | The answer is already known, or no actor would change behavior. |

## Self-Review Question List

Answer each with explicit evidence from the paper.

### 1. Identification

1. What is the source of variation, and where in the text is it defended?
2. Which selection threat matters most, and is a claimed bias direction supported?
3. Are filtering, trimming, and sample-construction rules stated in the open?
4. Were splits and estimands explained before body results that depend on them? Are introductory previews truthful?

### 2. Mechanism

1. Does the language distinguish identified mechanism effects from suggestive links and opposing channels?
2. When a rival is tested, is the result reported accurately, even if the test follows policy results?
3. Are non-causal links marked as such?
4. Does the net account explain the average while allowing individual channels to oppose it?

### 3. Results Ordering and Baselines

1. Does the field-experiment arc (including post-policy mechanism) or targeting prediction → model → counterfactual arc fit this paper's question?
2. Is each quantitative gain's comparator recoverable from the sentence or clear context?
3. Are train and test shown when the claimed generalization or learned-policy value requires them? Are fitted-sample checks labeled as such?
4. Are modest gains owned with a mechanical explanation?

### 4. Policy Evaluation

1. For a learned policy-value claim, is value independently estimated or supported by a suitable off-policy estimator? For structural counterfactuals, are fitted-sample checks and model assumptions labeled accurately?
2. Are the relevant comparators used, with a best-uniform test when that particular gap is claimed?
3. Are failing rival methods reported and diagnosed?
4. Are long-run consequences addressed where data exist?
5. Are scope conditions for transfer stated operationally?

### 5. Writing

1. Does each paragraph develop a coherent lesson, whether stated first or built from cases or formal objects?
2. Can a reviewer map each Abstract and Introduction claim to appropriate support, with a baseline only when applicable?
3. Are headline numbers substantively consistent, allowing compatible rounding?
4. Is any sentence long enough to need a second parse?

## Adversarial Workflow

1. Read the paper as a skeptical reviewer for the target journal.
2. Answer every question above with evidence from the paper.
3. Mark each applicable item `pass`, `needs revision`, or `needs new analysis`; otherwise mark `not applicable — reason`.
4. Revise claims, writing, analyses, or scope accordingly.
5. Repeat until no major rejection risk remains.

## Checklist

1. No dimension 1–3 risk remains open.
2. Every major Abstract and Introduction claim has an appropriate support entry in the reviewer’s map.
3. Every quantitative gain has a recoverable comparator and a clear evaluation basis where needed; details can be carried by nearby context.
4. Decisive scope conditions appear with bounded claims; broader limitations may appear in a later section.
5. Headline numbers agree in substance across sections, allowing compatible rounding.
6. Every item marked `needs new analysis` is either done or the claim it supports is weakened.
7. Flag every sentence a non-specialist must reread, parse through nested clauses, or look up a word to understand; check first-use definitions without dropping terms of art, numbers, or qualifications.
8. Every citation in the draft is verified to exist and supports its exact claim; every `[CITATION NEEDED: <the claim>]` placeholder is resolved or reported to the user.
9. For a multi-file LaTeX project, before declaring the revision complete, verify that the main file inputs/includes the edited section files; flag and synchronize any embedded duplicate text blocks, including those between marker comments.
10. Are identifying assumptions named in the identification argument and tied to the design feature or evidence that satisfies them? Flag separate assumption lists.
11. Is the main text self-contained? Flag any body passage that raises a substantive point and sends its examination, explanation, or specification to an online appendix.
