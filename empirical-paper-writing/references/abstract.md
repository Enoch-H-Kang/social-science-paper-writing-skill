# Abstract Writing Guide (Empirical Papers)

## Goal

An abstract in this genre is a compressed version of the whole argument. A reader who reads only the abstract should be able to repeat the paper's point at a seminar lunch, correctly, including the number. Two shapes cover most empirical papers: Version A (experiment to policy) and Version B (causal data plus an economic model).

## Pre-Writing Questions

Answer these before writing a word:

1. What does the firm, platform, or consumer actually do today, in one plain sentence?
2. Who are the actors, what are their objectives, and what constraint, tension, or debate matters? Name conflicting incentives when they exist.
3. What are the 2–3 research questions, as questions?
4. What are the components of the framework, and what counterfactual does each make computable?
5. What is the average effect, exactly, against which named baseline?
6. Which theory did you rule out, which did you support, and what result discriminates between them?
7. What is the personalized or optimal policy worth, evaluated how?
8. What will a manager or regulator do differently after this paper?

If questions 5–8 have no answer yet, the abstract is a promise, not a summary. Write the paper first.

## Version A: Experiment → Mechanism → Policy

Use when the paper has exogenous variation (a field experiment, a natural experiment, platform data with credible variation) and ends in a policy or design recommendation. One sentence per slot unless noted:

1. **Practice.** What firms in the industry actually do, in plain words.
2. **Design and variation.** "We use data from [a large-scale field experiment] to study the effect of [treatment] on [customer-level outcomes]."
3. **Average finding.** Flag it with "(surprisingly)" or an equivalent if it reverses the obvious guess.
4. **Mechanism verdict.** One theory ruled out, one supported, optionally a novel behavioral trace. One or two sentences.
5. **Policy construction.** "We then develop a [personalized policy / design] that assigns [treatment] to each [unit] based on [predictions]."
6. **Policy value.** Name the off-policy estimator and the gain: "[X%] improvement in [outcome] over [named status quo or uniform policy]."
7. **Long-run extension** (optional). Whether the short-run result survives in long-run outcomes.
8. **Heterogeneity as a who-gets-what rule.** Which segment should get which treatment.
9. **Cautionary or negative twist** (optional, powerful). Personalization does not always beat a simple uniform rule, and rival methods lose. The abstract may end on this scoped caution or negative comparison.
10. **Alternative implication.** When the paper supports a further actor rule, state what the actor should do. This is optional after a cautionary ending.

Fill-in skeleton: `examples/abstract-templates.md`.

## Version B: Causal Data + Economic Model → Policy/Incentives

Use when a measurement component built on large-scale causal or platform data is paired with an economic model to study market outcomes or regulation. Eight slots:

1. **Practice.** The market fact, with scale.
2. **The debate, naming its three objects:** the value of [information or design lever], the incentives of [actor] to [action], and the role of [regulation or design choice].
3. **Hinge.** "To answer these questions, we propose a unified framework with two components: [measurement component] and [economic model] for counterfactuals."
4. **Data** in one clause: scale and source.
5. **Headline number versus a named baseline.** Exact percentage.
6. **Decomposition.** Which ingredient carries the gain (for example behavioral versus contextual information).
7. **Incentive result.** The nonmonotonicity or reversal, stated as what the actor prefers.
8. **Implication for regulation or design,** when supported; a result, caution, or boundary may close instead.

Fill-in skeleton: `examples/abstract-templates.md`.

## Scope Placement

Name the setting early. Attach decisive conditions to the claims they bound, explain model assumptions in the setup, and gather broader limitations later. A framework may transfer beyond the setting even when the estimated finding does not; state the requirements for each separately.

## Sentence-Level Rules

1. Verbs do the work: *we use, we find, we show, we develop, we evaluate, we rule out*. No "leverages", "sheds light on", "delves into".
2. One finding per sentence. If a sentence holds two percentages for two findings, split it.
3. Every percentage names its baseline in the same sentence.
4. No citations, no notation, no acronym that the abstract does not itself define.
5. About 200 words is the ceiling. The cut comes from framework detail; keep the findings and the strongest supported close.
6. "Novel" appears at most once, attached to the framework, never to a finding.

## Checklist

1. Can a reader extract in one pass the practice, question, evidence, supported findings, and payoff or caution? Include mechanism and policy value when the paper establishes them.
2. Is every number baselined, and is every claim traceable to a result in the body?
3. Does the abstract end on its strongest supported payoff, finding, caution, boundary, or implication? Are decisive conditions attached to the claims they bound, wherever those claims appear?
4. Read aloud: does any sentence need a second parse? Split it.
