# Introduction Question-Set Template (Research Agenda, §1.2)

The signature move of the empirical introduction: numbered question sets, then challenges with named failures, then the mapping of components to challenges. Content is generic; replace brackets.

```latex
\subsection{Research Agenda}
% Question set 1: efficiency / the average effect
% Question set 2: the value of ingredients, or mechanism
% Question set 3: the tradeoff and incentives
% Challenges: counterfactual, prediction or estimation, incentive or structure
% Mapping: which component answers which challenge
```

## Question sets (three at most)

1. `The first set of questions relates to [efficiency / the average effect]: How can [actor] use [data] to [decision]? How can we evaluate [policies] in factual and counterfactual settings? What is the gain from [the efficient policy]?`
2. `The second set relates to the value of [ingredients]: What is the relative value of [A] versus [B]?`
3. `The third set relates to [the tradeoff and incentives]: What is the empirical relationship between [efficiency] and [actor's payoff]? Are the actors' incentives aligned?`

## Challenges

`There are [two/three] main challenges to answering these questions. First, [counterfactual challenge: we observe outcomes only for the option chosen, and [selection mechanism] makes the unobserved option's outcome impossible to infer without variation]. Second, [prediction or estimation challenge: a weak model of [outcome] biases the estimated value of [ingredient] [downward/upward]]. Third, [incentive or structure challenge: without a model of how [actors] respond, no statement about [payoff] is possible, however accurate the predictions].`

## Mapping sentence

`The first component addresses the first two challenges: it [estimates primitive] using [variation]. The second component addresses the third: it [imposes structure] so that [counterfactual outcomes] can be computed.`

## Checklist

1. At most three question sets, and every question is answered by a later section.
2. Every challenge names the failure that follows from ignoring it.
3. Every component maps to at least one challenge, and every challenge to a component.
4. Challenges describe what answering the question requires, not complaints about prior accuracy.
