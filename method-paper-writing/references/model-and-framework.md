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

For theory infrastructure, also ask which claimed result the component enables. A necessary definition, construction, or technical lemma may merit full treatment even when it is not a standalone economic contribution.

## Analytical / Game-Theoretic Model

For theorem statements, result dependencies, and proof writing, read [Theorem Statements and Proofs](theorem-and-proof-style.md). Use its characterization or equivalence route when that better fits the question than the candidate-equilibrium and benchmark sequence below.

**Source and variation.** The candidate-equilibrium, benchmark, main-result, comparative-static, and extension sequence follows the theory exemplar. Nearby interpretation recurs in the analytical hybrid. The numbered steps and proposition-by-objection structure are adaptable presentation aids.

1. **Make primitives intelligible.** Explain actors, objectives, information, timing, and relevant forces near their notation. A reader should be able to retell the game after the setup.
2. **Setup.** Introduce notation as needed, each symbol defined in the sentence that introduces it, with its economic meaning.
3. **Defend functional forms.** List the required properties, then choose the simplest form that satisfies them. Absorb objections into footnotes.
4. **Equilibrium concept and why it fits,** explained at the length the reader needs.
5. **Candidate equilibrium when applicable.** State the equilibrium you will verify, then verify it. For set characterizations or equivalence results, define the relevant objects and establish the supporting results needed for the headline claim.
6. **Benchmark model, when useful.** A no-X benchmark can clarify the main result; place it before the result it interprets.
7. **Propositions with nearby interpretation.** A plain-words explanation may precede or follow the formal statement. Use interpretive interludes when they clarify the economic force.
8. **Comparative statics with economic names.** Parameter, direction, and driving force; never bare monotonicity.
9. **The dichotomy check, when explaining two observed regimes.** Show the model generates both in different parameter regions. For other formal questions, check that the statement answers the question under its assumptions.
10. **Extensions** address the consequential objections or omitted features; formalize those that need a proposition. When an extension changes a substantive environment, objective, or benchmark, explain the relevant change and its consequence for the baseline claim. Where a preservation/change contrast clarifies the result, develop it using supported analysis or a labeled illustration. Brief portability or robustness extensions may use a short explanation and appendix pointer; do not require every slot or a fixed closing move.

## Structural / Estimation Framework

**Source and variation.** Decision states, selection, identification, estimates, fitted-sample checks, and counterfactuals follow the structural exemplar. Explaining consequential assumptions recurs across method papers. The exact state ordering and nested-model roster are source-specific options.

Open a multi-part model section with a compact roadmap paragraph mapping each modular block to its explicit subsection number (for example, §X.1, §X.2, §X.4.1).

1. **Model Setup: the decision as the agent faces it.** Before the institutional timeline, declare index sets (time $t \in \{1,\dots,T\}$ and population $i \in \{1,\dots,N\}$), formal decision notation ($d_{it}$), unit-of-observation equivalences ("with some abuse of notation"), and preferences over state sequences across $t = 1,\dots,T$. Keep agency centered on the modeled decision-maker, including the options to wait, cancel, or do nothing when these appear in the data; do not introduce non-modeled market sides as active subjects. Complete the abstract timing lifecycle first: period-1 start, each period's choice set with state-dependent feasibility hedges such as "(if any)," and terminal or expiry stopping conditions. Then mark empirical calibration explicitly: "In our data and analysis, one period is equivalent to [unit], and T = [value]."
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
3. **Material assumptions are identifiable, motivated, and connected to the claims they bound.** Explain what each rules out.
4. **Place conditions at their objects.** State each material condition once, in prose where the object it constrains is introduced, and explain in the same passage what it makes possible, identifies, or rules out. Do not collect conditions in an upfront list, an "Assumptions" section, or a summary paragraph that repeats conditions stated in subsections; duplication between a list and the body is a defect. Use a formal numbered assumption environment only when results in other sections need to cite the condition by a handle, and still state it at its object rather than in a separate upfront block.
5. **Consequential modeling choices** answer a challenge or trace to the institutional setting.
6. **Use measured restricted-version failures** when they help explain the full framework; label the tested comparison.
7. **Assemble model setup in the reader's building order.** Present environment and primitives first, weaving who observes what into the objects as they appear (observed before unobserved); then give the timeline or protocol. Present the objective or payoff as one component among the others under a plain component heading, never a question-form or evaluative heading. Stop at the environment: state objects without deriving consequences there, and give learning, estimation, and solution machinery its own section or place it with the results it serves.

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
