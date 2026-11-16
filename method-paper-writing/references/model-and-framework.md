# Model and Framework Writing Guide (Method Papers)

The core guide of this skill. A "method section" may present an analytical model, a structural or estimation framework, or an ML or algorithmic method. Explain primitives and economic meaning close to the formal objects, in either order.

## Pre-Writing Questions

For each component, answer in one line:

1. Which research question does it answer?
2. Which challenge does it overcome?
3. What is the key primitive it produces (a preference parameter, a policy, an equilibrium object, a prior)?
4. What counterfactual or characterization becomes computable once you have that primitive?
5. What assumption does it need, and what breaks if the assumption fails?

If a component has no answer to question 4, it is engineering, not a contribution. Describe it in one paragraph and move on.

## Analytical / Game-Theoretic Model

**Source and variation.** The candidate-equilibrium, benchmark, main-result, comparative-static, and extension sequence follows the theory exemplar. Nearby interpretation recurs in the analytical hybrid. The numbered steps and proposition-by-objection structure are adaptable presentation aids.

1. **Make primitives intelligible.** Explain actors, objectives, information, timing, and relevant forces near their notation. A reader should be able to retell the game after the setup.
2. **Setup.** Introduce notation as needed, each symbol defined in the sentence that introduces it, with its economic meaning.
3. **Defend functional forms.** List the required properties, then choose the simplest form that satisfies them. Absorb objections into footnotes.
4. **Equilibrium concept and why it fits,** explained at the length the reader needs.
5. **Candidate equilibrium first.** State the equilibrium you will verify, then verify it.
6. **Benchmark model, when useful.** A no-X benchmark can clarify the main result; place it before the result it interprets.
7. **Propositions with nearby interpretation.** A plain-words explanation may precede or follow the formal statement. Use interpretive interludes when they clarify the economic force.
8. **Comparative statics with economic names.** Parameter, direction, and driving force; never bare monotonicity.
9. **The dichotomy check, when explaining two observed regimes.** Show the model generates both in different parameter regions. For other formal questions, check that the statement answers the question under its assumptions.
10. **Extensions** address the consequential objections or omitted features; formalize those that need a proposition. When an extension changes a substantive environment, objective, or benchmark, explain the relevant change and its consequence for the baseline claim. Where a preservation/change contrast clarifies the result, develop it using supported analysis or a labeled illustration. Brief portability or robustness extensions may use a short explanation and appendix pointer; do not require every slot or a fixed closing move.

## Structural / Estimation Framework

**Source and variation.** Decision states, selection, identification, estimates, fitted-sample checks, and counterfactuals follow the structural exemplar. Explaining consequential assumptions recurs across method papers. The exact state ordering and nested-model roster are source-specific options.

1. **The decision as the agent faces it:** what is chosen each period, from what set, trading off what, including the options to wait, cancel, or do nothing when these appear in the data.
2. **State variables in a clear order:** distinguish observed from unobserved and time-invariant from time-varying where the model uses those distinctions.
3. **Where the bias lives.** Name the selection or dynamic problem and explain a direction only under assumptions that support it.
4. **Defend specification choices in paired alternatives:** the rejected option and why. Rule out non-modeled features with data-based reasons.
5. **Identification in prose** with a worked example; formal proof is deferred. Say which variation pins down each key parameter.
6. **Estimation in a replicator's order:** moments or objects, then the objective, then computation. Treat computational burden as narrative: justify each choice by tractability, with the infeasible alternative sketched.
7. **Use restricted models when they test a bias or fit claim.** Static or fewer-type variants can show what changes under the richer specification.
8. **Label model checks accurately.** Fitted-sample comparisons of predicted and observed choices are model checks; they are not independent held-out or untargeted validation. Use a holdout when the claim requires one.

## ML / Algorithmic Method

**Source and variation.** Tutorials, measured pure-approach diagnosis, a hybrid, and horizon comparisons follow the ML-method exemplar. Question-first motivation and calibrated performance claims recur across method papers. Primer length and benchmark roster are editorial adaptations.

1. **Estimand or task before algorithm:** define what is predicted or decided, and why it is the primitive the decision needs.
2. **Diagnosis as part one of the paper.** Each pure approach gets a tutorial, its actual configuration shown, and a result. Close with a verdict table and a cost comparison.
3. **The method as a modular framework** with a flagship instantiation: pseudocode, hyperparameters, and limiting cases that nest the incumbents (one setting recovers approach A, another recovers approach B). State honestly when formal guarantees are open.
4. **Tutorial generosity.** Give unfamiliar techniques enough explanation for a quantitatively sophisticated non-specialist; place intuition near the algorithm.
5. **Motivate design choices with business constraints:** cost, privacy, compatibility with existing systems.
6. **Benchmark roster** with a fair, disclosed protocol. Report tuning and the status-quo practice when those matter to the comparative claim.

## Writing Rules for All Three

1. **Economic explanation near formalism.** A definition, algorithm, or proposition may come first if interpretation follows closely and remains intelligible.
2. **One notation, everywhere.** Keep a notation table while drafting.
3. **Material assumptions are identifiable, motivated, and connected to the claims they bound.** Numbering is an option; explain what each rules out.
4. **Consequential modeling choices** answer a challenge or trace to the institutional setting.
5. **Use measured restricted-version failures** when they help explain the full framework; label the tested comparison.

## Clarity Check

1. Logic: summarize the section's argument in three sentences without notation.
2. Paragraph: develop a coherent lesson; cases or formal objects may appear before the conclusion.
3. Sentence: can you say why the reader needs it here? Keep definitions, tutorials, and reminders that help readers follow the main argument. Move alternative machinery to an appendix when its main-text appearance has no explanatory or scoping role. Remove or cross-reference repeated identities when the repetition adds no new interpretation or useful orientation; retain explanatory examples.

## Checklist

1. Does each component pass the five pre-writing questions?
2. Is the track-specific order followed (theory, structural, or ML)?
3. Is economic interpretation close enough to each important formal block to make it intelligible?
4. Is each material assumption findable, motivated, and connected to the claim it bounds?
5. Is the notation unique, with one symbol per object?
6. Are consequential modeling choices explained where they matter?
7. For an explanatory dichotomy, does the model generate both sides? For another formal result, does it answer its question under its assumptions? Are restricted models or limiting cases shown when the claimed comparison depends on them?
