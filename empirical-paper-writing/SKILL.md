---
name: empirical-paper-writing
description: Write and revise empirical papers for INFORMS-style journals (Management Science, Marketing Science, Journal of Marketing Research, Information Systems Research, QME) — field and natural experiments, causal analyses of platform or firm data, and papers that end in a policy or design evaluation. Start from a market puzzle, name the actors and the tradeoff, pose numbered research questions, treat identification as a main-text obligation, and report findings in the fixed order average effect → mechanism → heterogeneity → policy value, every gain quantified against a named baseline. Use when drafting or revising the Abstract, Introduction, Literature, Data/Identification, Results, or Conclusion of an empirical paper, or for a pre-submission adversarial review. Triggers: "write an empirical paper", "revise my field experiment paper", "empirical paper 써줘", "실증 논문 고쳐줘", "Management Science 스타일로 논문 써줘".
---

# Empirical Paper Writing

Adapted from Master-cai/Research-Paper-Writing-Skills (itself from Prof. Peng Sida's notes, MIT License). That package teaches ML/CV/NLP conference writing: teaser figure, pipeline, beat SOTA, ablate. This skill keeps its discipline (one paragraph = one message, reverse outlining, claim–evidence checks, adversarial self-review) and replaces its substance. The target is an empirical paper in the house style of quantitative marketing and management journals: a paper whose contribution is an answer about a market.

## Which skill should I use?

Classify the paper by where the headline contribution claim sits (the contribution sentence of the abstract). A market or policy answer means this skill. A tool (model, framework, estimator, algorithm) means the sibling skill, `method-paper-writing`, which covers analytical/game-theoretic models, structural estimation frameworks, and ML/econometric methods.

Hybrid papers use both skills and the primary one follows the headline.

- Headline is a market answer delivered through method components (an ML measurement step feeding an economic model, say): this skill is primary, and the method skill governs the component sections.
- Headline is the tool and the market answer is its payoff: the method skill is primary, and this skill governs the data and validation sections.

This skill works on its own. If the sibling is not installed, apply the track rules in this skill and say so when the paper's core is a tool.

## The One-Sentence Test

Before any sentence-level edit, the paper must pass this test in one breath:

> A named actor in a real market faces a decision. Reasonable people disagree about what they should do, because [tradeoff]. We answer [2–3 questions] with [framework], using [data / variation / model]. We find [average effect], because [mechanism, with the rival explanation ruled out]. This implies [a concrete policy or design], worth [quantified gain vs. a named baseline], and it flips the naive intuition that [X], because [incentive].

If any slot is empty, that is the paper's problem. Fix the slot, not the prose.

## Core Workflow

1. **Puzzle first.** State the market fact and the debate in plain language before any method. See `references/introduction.md`.
2. **Questions before framework.** Write the research questions as numbered questions, grouped in sets. Then list the 2–3 challenges that make them hard. The framework arrives as the answer to those challenges, component by component.
3. **Load only the section guide you need** (list below). Do not load all references at once.
4. **Rewrite paragraph by paragraph.** One message per paragraph; the first sentence states the message.
5. **Reverse-outline each section** after drafting: thesis → paragraph topic sentences → evidence under each. Delete or rewrite any paragraph that does not map.
6. **Run the claim map** (Output Contract). Every major claim in the Abstract and Introduction must point to an identified estimate, a mechanism test, or a policy evaluation, not to "the results table" in general.
7. **Run the adversarial review** in `references/paper-review.md` and revise until no high-risk item is open.

## The Ten Rules

1. **Start from what firms actually do, not from what methods cannot do.** The opening sentence is a plain fact about a market practice ("Trial offers are a common customer-acquisition strategy in subscription software"). Never open with a technical gap, a method name, or "recent advances in…".
2. **Name the actors and their conflicting incentives.** Advertisers vs. ad network vs. users vs. regulator; firm vs. sophisticated vs. unsophisticated consumers. A paper without a tension between named actors has no story yet.
3. **The puzzle is a tradeoff, and the title often names it.** Two nouns joined by "and" or "or". If you cannot state the tradeoff in two nouns, the contribution is not yet sharp.
4. **Prediction is not a contribution; the identified effect and the counterfactual are.** An ML model or an experiment earns its place by what it lets you compute that you could not observe: outcomes under a different policy, a different information regime, a different design. Pair the empirical component with an evaluation or economic component (policy-evaluation estimator, auction model) that carries the policy claim.
5. **Findings are reported in a fixed order: average → mechanism → heterogeneity → policy.** Average effect first, flagged if surprising. Then mechanism: rule one theory out, find support for another, with those verbs, not "we explore mechanisms". Then heterogeneity that is substantively interpreted. Then the designed policy and its value.
6. **Every gain is quantified against a named baseline.** A number, a denominator, a status quo with a name ("a 7% improvement over a uniform 30-day policy"). "Outperforms baselines" is banned.
7. **End on the incentive or behavior that flips.** The last finding should reverse a naive intuition (more targeting does not maximize revenue; a longer trial does not maximize conversion) or tell an actor what to do differently. If the ending is "our approach works better", rewrite it around what an actor will now choose.
8. **Intuition before math, always.** State the idea in plain words a smart non-specialist can repeat, then the formal version. State each contribution two ways: the technical answer, then the business perspective, ending in the simple rule a manager can run.
9. **Crisp is a quality standard.** Short declarative sentences, one finding per sentence, numbers inside the sentence, terms defined by what an actor does before they are defined by notation. Cut any sentence a reader must parse twice.
10. **Identification is a writing obligation, not a robustness footnote.** The source of variation, the selection problem, and the heterogeneity that could bias the headline number are named in the main text, where the estimate is introduced, with the direction of the bias.

## How this differs from ML-conference writing

| ML/CV conference | INFORMS journal |
|---|---|
| Technical challenge of prior methods | Market puzzle plus an unresolved debate among named actors |
| Pipeline or teaser figure as first impression | The question set and the tradeoff as first impression; figures serve the mechanism or the policy |
| Method = modules with motivation, design, advantage | Framework = components, each mapped to one research question and one identification challenge |
| Experiments = beat SOTA, ablate, harder settings | Results = average effect → mechanism discrimination → heterogeneity → policy evaluation with an off-policy estimator |
| Related work = competing methods grouped by technique | Literature = streams by substantive question and by method, each ending in what it cannot answer |
| Conclusion = restate, limitations, future work | Conclusion = managerial guideline + policy implication + scope conditions |
| Reviewer risk = weak gains, missing ablations | Reviewer risk = weak identification, undiscriminated mechanism, in-sample policy value, single-firm validity |

Keep from the conference tradition, unchanged: one paragraph, one message; topic sentence first; reverse outlining; stable terminology; weaken or delete any claim the evidence does not support; tables as communication (one table, one message; the caption states the setting and the takeaway).

## Section Guides

Load only the needed file from `references/`:

- Abstract: `references/abstract.md`
- Introduction: `references/introduction.md`
- Literature and positioning: `references/literature-and-positioning.md`
- Data, design and identification (core guide): `references/data-and-identification.md`
- Results: `references/results.md`
- Conclusion: `references/conclusion.md`
- Pre-submission review: `references/paper-review.md`
- Style evidence base: `references/style-evidence.md`
- Fill-in templates: `references/examples/abstract-templates.md`, `references/examples/introduction-question-set-template.md`, `references/examples/contribution-statement-template.md`

## Execution Rules

1. Build the question set and the claim map before drafting prose. Prose written before the questions exist gets discarded.
2. For each framework component, state in one line: which question it answers, which challenge it overcomes, which counterfactual it makes computable.
3. Never present the design as an improvement over a naive version of itself. Present it as the answer to the challenges, as if it had to be this way.
4. Mechanism claims require a discriminating test: a result one theory predicts and the rival does not. Correlation with a mediator is not a mechanism.
5. Evaluate policy value out of sample or with a bias-corrected off-policy estimator (such as inverse propensity scoring), and compare it to both the institutional status quo and the best uniform policy. In-sample policy value is not a reportable gain.
6. If a claim cannot be supported, weaken it in the Abstract and Introduction first; those are the two places reviewers punish overclaiming.
7. Keep the stakes concrete: name what is acquired, earned, or lost (customers who pay and customers who generate informative data; revenue, not "performance").

## Output Contract

When asked to draft or rewrite, return:

1. A compact outline (3–7 bullets) organized by research question, not by section boilerplate.
2. Revised paragraphs, each labeled with its role: `context / debate / question / challenge / approach / finding-average / finding-mechanism / finding-heterogeneity / policy / incentive-implication`.
3. A claim map for every major claim:
   `Claim: … | Support: identified estimate / mechanism test / policy evaluation | Baseline: … | Status: supported / needs evidence / overclaimed`
4. A short self-review: sentences to split or cut, intuition-before-math check, identification gaps, and any claim whose support is only in-sample.
