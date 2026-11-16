# Abstract Writing Guide (Empirical Papers)

## Goal

An abstract in this genre is a compressed version of the whole argument. A reader who reads only the abstract should be able to repeat the paper's point correctly. Two observed shapes offer starting points: Version A (experiment to policy) and Version B (causal data plus an economic model).

## Pre-Writing Questions

Answer these before writing a word:

1. What does the firm, platform, or consumer actually do today, in one plain sentence?
2. Who are the relevant actors, and what constraint, tension, or debate matters? Name conflicting incentives when they exist.
3. What research questions does this paper answer?
4. What are the components of the framework, and what counterfactual does each make computable?
5. What headline effect, predictive finding, or economic result is supported, and against what comparator when comparative?
6. What mechanism evidence exists: identified channel, suggestive link, opposing forces, or a tested rival?
7. What is the personalized or optimal policy worth, evaluated how?
8. What supported finding, caution, boundary, implication, or future question should close?

Answer the slots applicable to the paper; do not invent a mediator test or actor command to fill a template.

## Version A: Experiment → Mechanism → Policy

**Source and variation.** This slot sequence follows the field-experiment exemplar, including policy value before later heterogeneity. Market practice, supported findings, and careful qualification recur across both empirical exemplars. The sentence slots and optional actor implication are editorial adaptations.

Use when the paper has exogenous variation (a field experiment, a natural experiment, platform data with credible variation) and ends in a policy or design recommendation. One sentence per slot unless noted:

1. **Practice.** What firms in the industry actually do, in plain words.
2. **Design and variation.** "We use data from [a large-scale field experiment] to study the effect of [treatment] on [customer-level outcomes]."
3. **Average finding.** Flag it with "(surprisingly)" or an equivalent if it reverses the obvious guess.
4. **Mechanism evidence.** Report tested rivals when present; label suggestive associations and opposing channels at their actual strength.
5. **Policy construction.** "We then develop a [personalized policy / design] that assigns [treatment] to each [unit] based on [predictions]."
6. **Policy value.** Name the evaluation and the gain against its relevant comparator when a learned-policy value claim is made.
7. **Long-run extension** (optional). Whether the short-run result survives in long-run outcomes.
8. **Heterogeneity.** Report which segments benefit and how strongly the evidence supports an assignment rule.
9. **Cautionary or negative twist** (optional, powerful). Personalization does not always beat a simple uniform rule, and rival methods lose. The abstract may end on this scoped caution or negative comparison.
10. **Alternative implication.** When the paper supports a further actor rule, state what the actor should do. This is optional after a cautionary ending.

Fill-in skeleton: `examples/abstract-templates.md`.

## Version B: Causal Data + Economic Model → Policy/Incentives

**Source and variation.** The prediction/measurement and analytical-model hinge follows the targeting hybrid. Market-first motivation and calibrated quantitative comparisons recur in both empirical exemplars. The eight-slot compression and regulatory close are optional adaptations.

Use when a measurement component built on large-scale causal or platform data is paired with an economic model to study market outcomes or regulation. Eight slots:

1. **Practice and catalyst.** State the market fact, with scale, in one plain sentence. Follow with "Although these [ads / practices] have [property], they have raised concerns among [actor]."
2. **The debate, naming its three objects:** the value of [information or design lever], the incentives of [actor] to [action], and the role of [regulation or design choice].
3. **Hinge.** "To answer these questions, we propose a unified framework with two components: [measurement component] and [economic model] for counterfactuals."
4. **Data** in one clause: scale and source.
5. **Headline comparison.** A percentage and relevant baseline when a quantitative gain is claimed; compatible rounding is fine.
6. **Decomposition.** Which ingredient carries the gain (for example behavioral versus contextual information).
7. **Incentive result.** Enter counterfactuals directly, without an adversative "However," against the prediction gain; put the "although" contrast inside the counterfactual sentence. Keep the plain-language definition of "nonmonotonic" in that sentence, attached with "; that is,". State the positive revenue-maximizing regime in its own sentence: "Rather, it is maximized when..."
8. **Implication for regulation or design,** when supported; a result, caution, or boundary may close instead. When extrapolating from counterfactuals to a broader regulatory conclusion, prefer "Our results suggest that [actors] may have..." over "imply."

Fill-in skeleton: `examples/abstract-templates.md`.

## Scope Placement

Name the setting early. Attach decisive conditions to the claims they bound, explain model assumptions in the setup, and gather broader limitations later. A framework may transfer beyond the setting even when the estimated finding does not; state the requirements for each separately.

## Sentence-Level Rules

1. Verbs do the work: *we use, we find, we show, we offer, we develop, we evaluate, we rule out*. No "leverages", "sheds light on", "delves into". Use first-person possessives for the contributed method and final takeaways ("our framework," "our machine learning framework," "our results"), but leave standard analytical exercises unpossessed ("Theoretical and empirical counterfactuals show"). Do not stack reporting clauses in consecutive sentences ("We find that..." then "We further show that..."); let the phenomenon lead the follow-on decomposition ("These gains mainly stem from...").
2. Keep multi-finding sentences intelligible; split them when their logic becomes hard to follow.
3. State the comparator for a quantitative gain, in the sentence or clear nearby context.
4. No citations, no notation, no acronym that the abstract does not itself define.
5. About 200 words is the ceiling. The cut comes from framework detail; keep the findings and the strongest supported close.
6. Use novelty language only when the specific contribution is supported; no word quota is required.
7. When a regime label is an ordinary English verb or noun, such as `cloak` or `flaunt`, use it directly as a verb on first mention, without a parenthetical or quotation-mark gloss.

## Checklist

1. Can a reader extract in one pass the practice, question, evidence, supported findings, and payoff or caution? Include mechanism and policy value when the paper establishes them.
2. Is each quantitative gain compared with a recoverable baseline, and is every substantive claim traceable to appropriate support in the body?
3. Does the abstract end on its strongest supported payoff, finding, caution, boundary, or implication? Are decisive conditions attached to the claims they bound, wherever those claims appear?
4. Read aloud: does any sentence need a second parse? Split it.
