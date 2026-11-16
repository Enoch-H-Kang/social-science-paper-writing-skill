# Abstract Writing Guide (Method Papers)

## Goal

A method abstract compresses the argument: the dichotomy or decision problem, the failure of existing approaches, the offer, the primitive in plain words, the payload by track, and an actor-facing close. Three versions cover the three tracks.

## Pre-Writing Questions

1. What fails today, and how do you demonstrate it (proved, estimated, or benchmarked)?
2. What is the key primitive your tool builds?
3. What does the primitive make computable (a characterization, a counterfactual, a decision rule)?
4. Which track arc do the results follow?
5. What does the last sentence change for a named actor?

If questions 1 and 5 have no answer, the abstract is a promise, not a summary.

## Version T: Theory — Explain a Dichotomy or Price Delegation

Nine slots, in order:

1. **Opening, choose one:** **Observed dichotomy:** "There exists a dichotomy in [market]: some [actors] [action 1], whereas others [action 2]." **Price-of-delegation / mechanism-design decision problem:** [Actor] cannot fully specify [decision] in advance; [delegate] can profitably shortcut the agreed process; the paper prices or characterizes a mechanism that prevents the shortcut.
2. **Existing models cannot explain it,** in one sentence.
3. **The offer:** a model that explains the divide.
4. **Modeling premise in plain words:** the dual role or the two forces built in.
5. **Tradeoff, first half:** action 1 preserves [benefit X] but reduces [benefit Y].
6. **Tradeoff, second half,** as a mirrored sentence: action 2 undermines [X] but increases [Y]. Keep the pair parallel in structure.
7. **Conditions derived** under which each action occurs.
8. **Emergence or welfare bonus** a reader can repeat in one sentence (the best product endogenously becomes the hit).
9. **Optional implication** for an actor, without notation; carry its scope in the same sentence or the sentence before.

Template: `examples/abstract-template-theory.md`.

## Version S: Structural — Estimate and Counterfact

Ten slots:

1. **Setting** defined in a clause.
2. **Friction** (information asymmetry, search cost, uncertainty about quality).
3. **Debated remedy or open question.**
4. **Contribution = the framework.**
5. **The agent's per-period decision** (one sentence).
6. **Its tradeoffs** (one sentence).
7. **The bias hook:** ignoring [dynamics / selection] biases [parameter] [direction]; this framework handles it through [mechanism].
8. **Data** in one clause.
9. **Findings:** forward-looking behavior is present, and naive models are biased.
10. **Counterfactual payoff** in money or guidelines, with the scope of any actor-facing rule in the same sentence or the sentence before.

Template: `examples/abstract-template-structural.md`.

## Version M: ML Method — Diagnose and Hybridize

Eight slots:

1. **Managerial need.**
2. **Data and evaluation of the pure approaches** on a large real archive.
3. **Ranked negative result:** which pure approach does worst, which does best, and how far from useful.
4. **One-line verdict,** the empirical contribution in one sentence.
5. **Method announcement:** the named framework.
6. **Mechanism in one line:** how it fixes the pure approaches' failure modes.
7. **Win versus named baselines,** including the status-quo practice, with the boundary condition (the gain is largest when [scarce resource]).
8. **Scope and generalizability close.** Put any actor-facing rule and its scope in the same sentence or the sentence before.

Template: `examples/abstract-template-ml-method.md`.

## Sentence-Level Rules

1. Verbs do the work: *we use, we find, we show, we develop, we evaluate, we derive*. No "leverages", "sheds light on", "delves into".
2. One finding per sentence.
3. Every percentage names its baseline in the same sentence.
4. No citations, no notation, no undefined acronyms.
5. About 200 words is the ceiling; findings and the final implication are never the cut.
6. "Novel" appears at most once, attached to the framework.
7. State gains by regime.
8. The tool's name may appear once.
9. No theorem numbers in the abstract.

## Checklist

1. Is the version for the paper's track used, with no slots borrowed from another track?
2. Is the failure of existing approaches present?
3. Are the primitive and its payoff named?
4. Is the last sentence actor-facing, with its scope in that sentence or the one before it? Flag a close without one compact clause stating the conditions the rule depends on (information or record arrangement, payment or contract class, behavioral assumption, as applicable).
