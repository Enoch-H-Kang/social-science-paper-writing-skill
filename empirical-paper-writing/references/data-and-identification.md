# Data, Design and Identification Guide (Empirical Papers)

The core guide of this skill. It covers the setting, the design, the estimands, descriptive evidence, and identification.

## Goal

Identification is a writing obligation. The reader should find the source of variation and material selection threats in the main text. State a bias direction when it is supported; do not assign an unsupported sign.

## Setting and Institutions

**Source and variation.** The field experiment uses enrollment timing and treatment assignment; the targeting hybrid uses probabilistic allocation and filtering. Both explain variation in the main text. Numbered institutional steps and the split/estimand checklist are editorial options drawn chiefly from the field experiment's organization.

1. Describe the market and its mechanism as numbered steps (who moves first, what is shown, what is charged, what is observed).
2. Make institutional detail load-bearing: each fact underwrites a later assumption or estimand. Color that motivates nothing gets cut.
3. Anonymize transparently. State the transformation (for example, "dollar values are scaled by a constant").
4. Where possible, let the setting description double as the identification argument. A randomized or probabilistic allocation mechanism, once described, already answers half the selection question.

## The Design / The Variation

State the treatment arms or the natural variation, then defend the design against self-selection in prose.

1. Name the selection threat and explain the bias it could create. A directional example requires evidence for its premise and sign.
2. Then narrate the design feature that kills it (assignment revealed only after the trial starts, so assignment cannot influence the decision to enroll).
3. Close by naming the conditions a clean design needs, and say which are guaranteed by design and which are checked.

For observational data:

- State the filtering or trimming rule in the open. Hiding it reads as cherry-picking.
- Show propensity and covariate-balance evidence.
- State positivity and unconfoundedness in the setting's own vocabulary ("every impression had a non-zero chance of showing every eligible ad"), then note where the design makes them automatic.

## Estimands and Outcomes

1. Define each outcome operationally in a numbered list, including edge cases (what counts as a conversion if the user upgrades after the window closes?).
2. If the paper uses a novel behavioral construct (a pattern of inactivity, a usage-intensity measure), define it and diagram it before using it.
3. Declare train/test or estimation/holdout splits before interpreting the body results that depend on them. Truthful abstract and introduction previews may appear earlier.

## Descriptive Evidence Before Structure

1. Present model-free facts that establish that the phenomenon plausibly exists.
2. Hedge them explicitly as suggestive; they are not identified effects.
3. Choose descriptives that foreshadow the later estimation, so the reader meets each variable and pattern twice, first as a fact and later as an input.

## Identification, Argued in Words

Give identification its own short subsection in plain language.

1. What variation pins down each key parameter or effect?
2. What would not be identified without it?
3. What unobserved heterogeneity could bias the headline number, and is its direction known?
4. What are the honest limits (a single firm, a single time window, short-run outcomes)?
5. Name identifying assumptions in prose within the identification argument, each tied to the design feature or evidence that satisfies it (for example, random assignment establishes unconfoundedness by construction); do not isolate them in a separate assumptions list.

Attach decisive limits to the estimate and gather broader limitations in a later section when useful.

## Checklist

1. Is each threat named before the fix that addresses it?
2. Is any stated bias direction supported, and are unsigned threats explained honestly?
3. Are splits declared before body results that rely on them, while introductory previews remain truthful?
4. Is every institutional fact load-bearing for a later assumption or estimand?
5. Are filtering and trimming rules stated in the open?
6. Is descriptive evidence hedged as suggestive?
7. Are estimands and outcomes operational, with edge cases listed?
8. Is any anonymization transformation stated transparently?
