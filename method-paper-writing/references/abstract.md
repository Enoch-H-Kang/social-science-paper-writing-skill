# Abstract Writing Guide (Method Papers)

## Goal

A method abstract compresses the argument: the observed pattern, decision problem, or capability sought; the question or obstacle; the offer and its primitive in plain words; and the supported result. The track versions are starting points, not sentence obligations. End on the strongest supported result, payoff, caution, boundary, or implication.

## Pre-Writing Questions

1. What question or obstacle motivates the tool? If an existing approach fails, what evidence establishes that failure?
2. What is the key primitive your tool builds?
3. What does the primitive make computable or possible (a characterization, a counterfactual, a decision rule, or a capability)?
4. Which track arc do the results follow?
5. What result, payoff, caution, boundary, or implication best closes the abstract?

If questions 1 and 5 have no answer, the abstract is a promise, not a summary.

## Version T: Theory — Explain a Dichotomy, Price Delegation, or Enable a Capability

Choose the route that fits the formal question. The first route has nine slots:

1. **Observed dichotomy:** "There exists a dichotomy in [market]: some [actors] [action 1], whereas others [action 2]."
2. **Existing models cannot explain it,** in one sentence.
3. **The offer:** a model that explains the divide.
4. **Modeling premise in plain words:** the dual role or the two forces built in.
5. **Tradeoff, first half:** action 1 preserves [benefit X] but reduces [benefit Y].
6. **Tradeoff, second half,** as a mirrored sentence: action 2 undermines [X] but increases [Y]. Keep the pair parallel in structure.
7. **Conditions derived** under which each action occurs.
8. **Emergence or welfare bonus** a reader can repeat in one sentence (the best product endogenously becomes the hit).
9. **Optional implication** for an actor, without notation.

**Delegation route:** Begin with the decision an actor cannot fully specify, identify the delegate's possible shortcut, state the open pricing or mechanism-design question, introduce the mechanism and its decisive property, then give the formal result and its conditions. Add an actor implication only when the result supports one. This route does not require two observed actions or an emergence result.

**Optional capability/enabling route (theorem adaptation is an extrapolation):** The source corpus shows enabling-method rhetoric, but no sufficiency or equivalence abstract template. Use this seven-slot sequence when the paper's actual theorem is about what a construction makes possible:

1. **Task or capability sought:** what an actor or analyst wants to accomplish.
2. **Open feasibility or adequacy question:** what remains unestablished for the identified setting or comparator. Claim a demonstrated failure only when one exists.
3. **Setup and enabling property:** relevant information, resources, or procedure and the property that makes the construction work, in plain words.
4. **Main formal result:** what is sufficient, necessary, or equivalent, and for which outcome. Do not turn sufficiency into equivalence or an asymptotic result into a finite-resource claim.
5. **Reason or intuition:** why the property yields the result; merge this with slot 3 when clearer.
6. **Scope or boundary:** attach decisive conditions to the setup or result they bound; use a separate sentence only if it adds information.
7. **Optional closing payoff:** an enabled task, theoretical consequence, practical implication, or unresolved boundary supported by the paper.

Merge slots when the argument reads more clearly that way. This route requires no opposing actions, mirrored tradeoff, numerical superiority, welfare bonus, or failed incumbent.

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
10. **Counterfactual payoff** in money or guidelines, qualified where the inference depends on a condition.

Template: `examples/abstract-template-structural.md`.

## Version M: ML Method — Diagnose and Hybridize

Eight slots:

1. **Managerial need.**
2. **Data and evaluation of the pure approaches** on a large real archive.
3. **Ranked negative result:** which pure approach does worst, which does best, and how far from useful.
4. **One-line verdict,** the empirical contribution in one sentence.
5. **Method announcement:** the named framework.
6. **Mechanism in one line:** how it addresses the tested approaches' limitations.
7. **Result versus named baselines tested,** including the status-quo practice when evaluated; identify the regime where the advantage is supported.
8. **Scope or generalizability close,** if supported; a result or caution may close instead.

Template: `examples/abstract-template-ml-method.md`.

## Scope Placement

Name the setting early. Attach decisive conditions to the claims they bound, state model assumptions where the setup needs them, and gather broader limitations later. A framework may transfer to another setting even when a particular finding does not; state the requirements for each separately.

## Sentence-Level Rules

1. Verbs do the work: *we use, we find, we show, we develop, we evaluate, we derive*. No "leverages", "sheds light on", "delves into".
2. One finding per sentence.
3. Every percentage names its baseline in the same sentence.
4. No citations, no notation, no undefined acronyms.
5. About 200 words is the ceiling; keep the findings and the strongest supported close.
6. "Novel" appears at most once, attached to the framework.
7. State quantitative gains by regime when the result makes such a comparison.
8. The tool's name may appear once.
9. No theorem numbers in the abstract.

## Checklist

1. Does the chosen route fit the paper's actual question and result? Borrow a useful slot from another route when it improves that fit.
2. Is the motivating question or obstacle established at the strength the evidence warrants?
3. Are the primitive and its payoff named?
4. Does the close state the strongest supported result, payoff, caution, boundary, or implication? Are decisive conditions attached to the claims they bound, wherever those claims appear?
