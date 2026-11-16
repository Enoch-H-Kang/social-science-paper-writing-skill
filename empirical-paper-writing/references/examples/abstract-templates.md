# Abstract Templates (Empirical Papers)

Two fill-in skeletons. Content below is generic and invented; replace every bracket.

## Version A: Experiment → Mechanism → Policy

```latex
\section{Abstract}
% Practice: what firms in the industry actually do
% Design + variation: the experiment and the outcomes
% Average finding (flag a surprise)
% Mechanism verdict: ruled out / supported / novel trace
% Policy construction: who gets what, based on what predictions
% Policy value: named off-policy estimator, X% vs. a named baseline
% Long-run extension (optional)
% Heterogeneity as a who-gets-what rule
% Cautionary twist (optional): may close on a scoped negative comparison
% Alternative implication for an actor (optional after a cautionary close)
```

## Reusable skeleton A

1. `[Practice sentence: what firms in INDUSTRY actually do.]`
2. `We use data from [a large-scale field experiment / N users on PLATFORM] to study the effect of [treatment] on [outcomes].`
3. `We find that [average finding] (surprisingly), [short clause on the obvious guess it reverses].`
4. `We rule out [theory 1], find support for [theory 2], and document [novel behavioral trace].`
5. `We then develop a [personalized policy] that assigns [treatment] to each [unit] using [predictions from a named learner].`
6. `Evaluated with [named off-policy estimator], the policy raises [outcome] by [X%] relative to [named status-quo or uniform policy].`
7. `[Optional: In the long run, [result on long-run outcome].]`
8. `[Segment A] should receive [treatment 1], whereas [segment B] should receive [treatment 2].`
9. `[Optional: However, [rival methods] fail to beat [simple uniform rule], because [diagnosis].]`
10. `[Optional alternative close: [Actor] should [concrete guideline supported by the result].]`

## Version B: Causal Data + Economic Model → Policy/Incentives

```latex
\section{Abstract}
% Practice with scale
% The debate and its three objects
% Hinge: two components
% Data in one clause
% Headline number vs. named baseline
% Decomposition: which ingredient carries the gain
% Incentive result: the reversal
% Implication for regulation or design
```

## Reusable skeleton B

1. `[Practice sentence with scale: PLATFORMS now carry X% of PRACTICE.]`
2. `Debate centers on [value of INFORMATION OR LEVER], [ACTOR]'s incentives to [action], and the role of [regulation or design choice].`
3. `To answer these questions, we propose a unified framework with two components: [measurement component] and [economic model] for [counterfactuals].`
4. `We apply it to [large-scale data from PLATFORM in MARKET].`
5. `[Measurement component] improves [outcome] by [X%] over [named baseline].`
6. `The gains stem mainly from [ingredient A]; the value of [ingredient B] is small.`
7. `[Actor outcome 1] rises monotonically with [lever], but [actor outcome 2] peaks when [condition], so [actor] prefers [choice].`
8. `[Actor] may therefore have economic incentives to [action] without [external intervention].`

## Usage rules

1. Reuse the sentence logic, not the wording. Rewrite each slot in the paper's own vocabulary.
2. Every number slot carries a baseline slot in the same sentence.
3. Delete optional slots cleanly; never leave a transition that referred to the removed slot.

## Checklist

1. Does every number slot carry a named baseline in the same sentence?
2. Is the version chosen by the paper's shape (experiment to policy, or causal data plus an economic model)?
3. Does the last sentence carry the strongest supported payoff, finding, caution, boundary, or implication, with decisive conditions attached to the claims they bound?
4. Do the optional slots you kept all have support in the body?
