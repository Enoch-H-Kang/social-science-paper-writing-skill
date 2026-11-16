# Introduction Writing Guide (Empirical Papers)

## Goal

The introduction does in about four pages what the abstract does in one paragraph, but it must earn each step: the reader should feel the debate is real, the questions are the right ones, the challenges are hard, and the framework is the natural answer. The strongest introductions in these journals split explicitly into context / agenda and challenges / approach / findings.

## Backward Reasoning First

Answer before writing:

1. What decision does a named actor face, and what observed practice or unresolved question motivates it?
2. What are the actors' objectives and the relevant constraint or tension? Are incentives actually in conflict?
3. What are the research questions, grouped into at most three sets?
4. For each question, what makes it hard: which variation, prediction, or economic structure is missing?
5. What does each framework component deliver, and which challenge does it map to?
6. Findings in order: average → mechanism → heterogeneity → policy value → incentive implication.
7. Against which two literatures does the paper position itself, one substantive and one methodological, and what can neither answer?

## Section Skeleton

```latex
\section{Introduction}
% 1.1 Context: the practice, the actors, the stakes (short)
% 1.2 Research agenda: numbered question sets, then the challenges
% 1.3 Our approach: the framework, component by component, mapped to challenges
% 1.4 Findings and contributions: results in order, then contributions by literature
% Roadmap (optional; drop it if the findings preview walks the paper's order)
```

## 1.1 Context: The Practice and the Tension

1. Open with scale or prevalence from the market, not the literature: what share of spend, how many firms, how common the practice.
2. Explain why the practice exists: what it lets the actor do.
3. State the relevant constraint, opposing effect, or conflict. Name an opposing actor only when the setting has one.
4. Close with the knowledge gap stated as a missing understanding, not a missing method, followed by the questions it blocks.

Rules: keep it short (past about 1.5 pages, institutional detail belongs in the data section); every fact is load-bearing for a later question; no academic citations in the first paragraph. A motivating data figure inside the introduction is a legitimate power move when a challenge (dynamics, selection) can be shown rather than asserted.

## 1.2 Research Agenda and Challenges

The signature subsection, written in two moves.

**Move 1: question sets.** State the questions as questions, grouped, three sets at most. The explicit numbered research-question list is the signature move: 3–5 questions, escalating, and every one answered by a later section. Reviewers check the mapping. A question no later section answers is deleted here.

**Move 2: challenges.** "There are three main challenges to answering these questions." Each challenge names the failure that follows from ignoring it:

- Counterfactual challenge: decisions need outcomes for options not chosen; without exogenous variation the counterfactual set may be empty.
- Prediction challenge: with a weak predictive model the estimated value of information or design is biased (state the direction, usually downward).
- Incentive challenge: without an economic model of strategic interaction, no statement about any actor's incentives is possible, however good the predictions.

Challenges are about what answering the question requires, not about beating a benchmark.

## 1.3 Our Approach

Introduce the framework as the direct answer to the challenges, in the same order.

1. "We present a unified framework that combines [empirical component] with [economic component]. It has [two/three] components."
2. Component 1 in one short paragraph: what it estimates, the key primitive it produces, which challenges it addresses.
3. Component 2: what structure it imposes, what it lets you compute under counterfactual regimes, which challenge it addresses.
4. Data and setting in one paragraph, which is really an identification paragraph: why this setting contains the variation the challenges require.

Rules: name the primitives; sell each component by the counterfactual it unlocks, not by adjectives; for a standard learner or estimator, say so in one clause and spend the words on why it is the right tool.

## 1.4 Findings and Contributions

**Findings.** Previewing essentially all results quantitatively is the norm in this genre (unlike an ML-conference teaser). One short paragraph or less each, in the fixed order:

1. Average effect: exact number, named baseline, surprise flagged.
2. Mechanism verdict: what was ruled out, what was supported, the discriminating result in one clause.
3. Heterogeneity, as a rule a manager could use.
4. Policy value: the policy, the evaluation method, the gain over the status quo and over the best uniform policy.
5. Incentive or behavioral implication, stated plainly.

Own modest gains with a mechanical explanation. A negative result can get equal billing.

**Contributions.** Use short paragraphs for the relevant audiences (substantive, methodological, managerial or policy), ordered by the paper's headline. Contrast closest work when a source supports the precise difference; the contrast need not end each paragraph. See `examples/contribution-statement-template.md`.

## Roadmap

Optional. When the findings preview already walks the paper's order, drop it. Otherwise two or three sentences: section numbers and one-line contents.

## Anti-Patterns

1. Opening with the literature ("A growing body of work studies…"). The market opens.
2. Opening with the method before the decision problem exists.
3. A challenges paragraph that is a complaint about prior papers' accuracy.
4. Findings listed in the order the analyses were run.
5. Contribution bullets that repeat the findings in new words. Findings say what is true; contributions say what the field can now do or know.
6. A paragraph whose first sentence does not state its message.

## Checklist

1. Could a reader who stops after 1.2 state the paper's questions and why they are hard?
2. Does every component map to a named challenge, and every question to a findings paragraph?
3. Are the findings in the fixed order, each with its number and baseline?
4. Is the incentive or behavioral implication present, and is it the last finding?
5. Reverse outline: thesis → topic sentences → evidence. Is anything unmapped?

## Scope Placement

Identify the setting before drawing inferences. Put decisive conditions beside the claims they bound, explain material model assumptions with the setup, and gather other limitations later. A transferable framework may support context-dependent findings; distinguish the requirements for applying the framework from the conditions under which a result transfers.
