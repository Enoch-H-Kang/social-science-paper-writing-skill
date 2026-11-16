# Model and Framework Writing Guide (Method Papers)

The core guide of this skill. A "method section" is one of three things, an analytical model, a structural or estimation framework, or an ML or algorithmic method. All three are written primitives-first and intuition-first.

## Pre-Writing Questions

For each component, answer in one line:

1. Which research question does it answer?
2. Which challenge does it overcome?
3. What is the key primitive it produces (a preference parameter, a policy, an equilibrium object, a prior)?
4. What counterfactual or characterization becomes computable once you have that primitive?
5. What assumption does it need, and what breaks if the assumption fails?

If a component has no answer to question 4, it is engineering, not a contribution. Describe it in one paragraph and move on.

## Analytical / Game-Theoretic Model

1. **Primitives in words first.** Actors, wants, information, timing of moves, and the two forces in tension, all before notation. A reader should be able to retell the game after one page.
2. **Setup.** Introduce notation as needed, each symbol defined in the sentence that introduces it, with its economic meaning.
3. **Defend functional forms.** List the required properties, then choose the simplest form that satisfies them. Absorb objections into footnotes.
4. **Equilibrium concept and why it fits,** in two sentences.
5. **Candidate equilibrium first.** State the equilibrium you will verify, then verify it.
6. **Benchmark model.** The no-X benchmark gives the main behavior its meaning as a deviation from it; present it before the main result.
7. **Propositions with intuition first.** Plain-words statement of what happens, for whom, and why, adjacent to the formal statement. Proofs go to the appendix unless the proof is the intuition. Use italic-titled interpretive interludes to name the economic concept a result instantiates.
8. **Comparative statics with economic names.** Parameter, direction, and driving force; never bare monotonicity.
9. **The dichotomy check.** Show the model generates both observed regimes in different parameter regions.
10. **Extensions** are the three most obvious objections, each preempted with its own proposition, each extracting new insight.

## Structural / Estimation Framework

1. **The decision as the agent faces it:** what is chosen each period, from what set, trading off what, including the options to wait, cancel, or do nothing when these appear in the data.
2. **State variables in a fixed order:** observed and unobserved, each split into time-invariant and time-varying. Introduce unobservables with concrete behavioral stories.
3. **Where the bias lives.** Name the selection or dynamic problem here, not in robustness: which unobserved heterogeneity exists and which way ignoring it biases the headline parameter.
4. **Defend specification choices in paired alternatives:** the rejected option and why. Rule out non-modeled features with data-based reasons.
5. **Identification in prose** with a worked example; formal proof is deferred. Say which variation pins down each key parameter.
6. **Estimation in a replicator's order:** moments or objects, then the objective, then computation. Treat computational burden as narrative: justify each choice by tractability, with the infeasible alternative sketched.
7. **Keep nested inferior models** (static, fewer types) estimated and on stage so the bias claim is demonstrated, not asserted.
8. **Fit and validation** against untargeted or held-out moments, stated before any counterfactual.

## ML / Algorithmic Method

1. **Estimand or task before algorithm:** define what is predicted or decided, and why it is the primitive the decision needs.
2. **Diagnosis as part one of the paper.** Each pure approach gets a tutorial, its actual configuration shown, and a result. Close with a verdict table and a cost comparison.
3. **The method as a modular framework** with a flagship instantiation: pseudocode, hyperparameters, and limiting cases that nest the incumbents (one setting recovers approach A, another recovers approach B). State honestly when formal guarantees are open.
4. **Tutorial generosity.** Assume a quantitatively sophisticated reader who is not an ML specialist: a two-paragraph primer plus intuition for every borrowed technique.
5. **Motivate design choices with business constraints:** cost, privacy, compatibility with existing systems.
6. **Benchmark roster** with disclosed tuned grids and a fair protocol, including the status-quo practice.

## Writing Rules for All Three

1. **Intuition paragraph before formalism** at the top of every model or framework section: five to eight lines, no notation, that a coauthor from another field could repeat.
2. **One notation, everywhere.** Keep a notation table while drafting.
3. **Assumptions are numbered, named, and motivated by the setting,** with one sentence on what each rules out.
4. **Every modeling choice answers a challenge** or traces to the institutional setting.
5. **Never write the framework as an improvement over a naive version of itself.**

## Clarity Check

1. Logic: summarize the section's argument in three sentences without notation.
2. Paragraph: the first sentence states the message; one paragraph, one message.
3. Sentence: can you say why the reader needs it here? Sentences that exist "for completeness" move to the appendix.

## Checklist

1. Does each component pass the five pre-writing questions?
2. Is the track-specific order followed (theory, structural, or ML)?
3. Does an intuition paragraph precede every formal block?
4. Is each assumption numbered, motivated, and paired with what it rules out?
5. Is the notation unique, with one symbol per object?
6. Is every modeling choice defended on the spot?
7. Does the model generate both sides of the phenomenon (theory), or are the nested inferior models kept on stage (structural), or do limiting cases nest the incumbents (ML)?
