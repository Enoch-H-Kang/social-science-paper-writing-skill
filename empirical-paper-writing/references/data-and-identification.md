# Data, Design and Identification Guide (Empirical Papers)

The core guide of this skill. It covers the setting, the design, the estimands, descriptive evidence, and identification.

## Goal

Identification is a writing obligation. The reader must find, in the main text and where the estimate is introduced, the source of variation, the selection threat, and the direction of the potential bias.

## Setting and Institutions

1. Describe the market and its mechanism as numbered steps (who moves first, what is shown, what is charged, what is observed).
2. Make institutional detail load-bearing: each fact underwrites a later assumption or estimand. Color that motivates nothing gets cut.
3. Anonymize transparently. State the transformation (for example, "dollar values are scaled by a constant").
4. Where possible, let the setting description double as the identification argument. A randomized or probabilistic allocation mechanism, once described, already answers half the selection question.

## The Design / The Variation

State the treatment arms or the natural variation, then defend the design against self-selection in prose.

1. Name the threat abstractly first, with the bias that follows ("users who self-select into longer trials are likely more engaged, which would overstate the effect").
2. Then narrate the design feature that kills it (assignment revealed only after the trial starts, so assignment cannot influence the decision to enroll).
3. Close by naming the conditions a clean design needs, and say which are guaranteed by design and which are checked.

For observational data:

- State the filtering or trimming rule in the open. Hiding it reads as cherry-picking.
- Show propensity and covariate-balance evidence.
- Restate positivity and unconfoundedness in the setting's own vocabulary ("every impression had a non-zero chance of showing every eligible ad"), then note where the design makes them automatic.

## Estimands and Outcomes

1. Define each outcome operationally in a numbered list, including edge cases (what counts as a conversion if the user upgrades after the window closes?).
2. If the paper uses a novel behavioral construct (a pattern of inactivity, a usage-intensity measure), define it and diagram it before using it.
3. Declare train/test or estimation/holdout splits here, before any result. A split announced after results looks tuned.

## Descriptive Evidence Before Structure

1. Present model-free facts that establish that the phenomenon plausibly exists.
2. Hedge them explicitly as suggestive; they are not identified effects.
3. Choose descriptives that foreshadow the later estimation, so the reader meets each variable and pattern twice, first as a fact and later as an input.

## Identification, Argued in Words

Give identification its own short subsection in plain language.

1. What variation pins down each key parameter or effect?
2. What would not be identified without it?
3. What unobserved heterogeneity could bias the headline number, and in which direction?
4. What are the honest limits (a single firm, a single time window, short-run outcomes)?

State limits here, with the estimate, rather than quarantining them in a final limitations section.

## Checklist

1. Is each threat named before the fix that addresses it?
2. Is the direction of potential bias stated for each threat?
3. Are splits declared before any result?
4. Is every institutional fact load-bearing for a later assumption or estimand?
5. Are filtering and trimming rules stated in the open?
6. Is descriptive evidence hedged as suggestive?
7. Are estimands and outcomes operational, with edge cases listed?
8. Is any anonymization transformation stated transparently?
