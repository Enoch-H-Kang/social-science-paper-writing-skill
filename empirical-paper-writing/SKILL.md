---
name: empirical-paper-writing
description: Write and revise empirical papers aimed at quantitative marketing and management journals — field and natural experiments, causal analyses of platform or firm data, and policy or design evaluations. Start from a market question, explain relevant actors and variation, calibrate findings to their evidence, and choose a results arc that fits the question. Use when drafting or revising the Abstract, Introduction, Literature, Data/Identification, Results, or Conclusion of an empirical paper, or for a pre-submission review. Triggers: "write an empirical paper", "revise my field experiment paper", "empirical paper 써줘", "실증 논문 고쳐줘", "Management Science 스타일로 논문 써줘".
---

# Empirical Paper Writing

Adapted from an MIT-licensed research-paper-writing package. The target is an empirical paper whose main contribution answers a market question. The sampled venues are Management Science and Marketing Science; other journals named in the description are target venues, not sampled evidence. Reverse outlines, claim maps, role labels, prose quotas, review loops, and LaTeX assembly checks are general editorial aids, not documented drafting practice in the sampled papers.

## Which skill should I use?

Classify by the paper's question and hierarchy of contributions across the abstract and introduction. A market or policy answer favors this skill; a tool developed as the main contribution favors `method-paper-writing`. A model or framework named in an abstract does not alone determine the primary route.

Hybrid papers use both skills and the primary one follows the headline.

- Headline is a market answer delivered through method components (an ML measurement step feeding an economic model, say): this skill is primary, and the method skill governs the component sections.
- Headline is the tool and the market answer is its payoff: the method skill is primary, and this skill governs the data and validation sections.

This skill works on its own. If the sibling is not installed, apply the track rules in this skill and say so when the paper's core is a tool.

## The One-Sentence Test

Before any sentence-level edit, the paper must pass this test in one breath:

> A named actor in a real market faces [decision] under [relevant constraint or tension]. We answer [research questions] with [design or framework], using [data / variation / model]. We find [supported effects and mechanisms]. This implies [policy, caution, boundary, or other payoff], with [quantified gain versus a named baseline] when a gain is claimed.

Use the slots that match the paper's claims. If a necessary answer is missing, fix the argument before polishing prose.

## Core Workflow

1. **Puzzle first.** State the market fact and the debate in plain language before any method. See `references/introduction.md`.
2. **Questions before framework.** Write the research questions as numbered questions, grouped in sets. Then list the 2–3 challenges that make them hard. The framework arrives as the answer to those challenges, component by component.
3. **Load only the section guide you need** (list below). Do not load all references at once.
4. **Rewrite paragraph by paragraph.** Keep each paragraph coherent; a case or formal object may come first and its lesson may emerge later in the paragraph.
5. **Reverse-outline each section** after drafting: thesis → paragraph topic sentences → evidence under each. Delete or rewrite any paragraph that does not map.
6. **Run the claim map** (Output Contract). Match each major claim to its appropriate support: an identified estimate, policy evaluation, sourced institutional fact, documented case, analytical proof, explicitly suggestive descriptive, or implementation argument. Evaluate each at its stated strength.
7. **Run the adversarial review** in `references/paper-review.md` and revise until no high-risk item is open.

## The Ten Rules

1. **Start from the market question.** A plain fact about a market practice can open the paper ("Trial offers are a common customer-acquisition strategy in subscription software"). Measured prediction or method failures can also motivate the question when their evidence and scope are clear.
2. **Name the actors, objectives, and relevant constraint or tension.** Describe conflicting incentives when they exist; opposing effects or an unresolved decision can also motivate the paper.
3. **State the decision tension plainly.** A two-noun tradeoff can work when the paper has one; an open design decision or opposing effects may call for a different formulation.
4. **Connect prediction to the economic question.** Prediction can be a methodological contribution; explain what it enables and support policy or incentive claims with the appropriate evaluation or model.
5. **Choose a results arc that fits the question.** The field-experiment exemplar moves from average effects and mechanisms to policy design/value, then returns to segmentation and mechanism before long-run outcomes. The targeting hybrid moves from prediction and targeting value to an analytical model and market counterfactuals. Mechanism evidence may identify a channel, support it suggestively, or show opposing forces; use the corresponding strength of language.
6. **Baseline comparative gains.** Give the number and comparator where a quantitative improvement is claimed; context may carry the comparator into later sentences. Qualitative findings and absolute quantities do not require invented percentages.
7. **End on the strongest supported finding, caution, boundary, or implication.** State an incentive reversal or actor rule when the evidence supports one; qualify the claim where it appears.
8. **Keep economic explanation near the math.** A formal definition or proposition may precede its plain-language interpretation. Give the practical perspective when relevant and supported.
9. **Crisp is a quality standard.** Short declarative sentences, one finding per sentence, numbers inside the sentence, terms defined by what an actor does before they are defined by notation. Cut any sentence a reader must parse twice.
10. **Explain identification in the main text.** Name the source of variation and material selection threats. State a bias direction when the evidence supports one; do not invent its sign.

## Empirical paper choices

| Question or evidence | Useful presentation choice |
|---|---|
| Market practice or decision | Explain the unresolved question and relevant actors |
| Several question sets | Map each to the needed variation, prediction, or economic structure |
| Field experiment with policy learning | Average effects and mechanisms → policy value → segmentation and further mechanism → long-run outcomes, when available |
| Prediction feeding an economic model | Prediction → targeting value → analytical model → market counterfactuals |
| Literature | Use the substantive and methodological streams the question needs, including four or five streams when warranted |
| Conclusion | Close on a supported finding, caution, implication, boundary, or future question |
| Review | Check identification, evidence strength, evaluation appropriate to each claim, and scope |

Keep terminology stable, make tables intelligible, and weaken claims that exceed their evidence.

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
3. Measured failures of restricted or naive versions can motivate the design; state the tested setting and scope of the comparison.
4. Report mechanism evidence at its strength. Distinguish identified mediation from suggestive associations, and explain opposing channels without requiring a rejected-rival scorecard.
5. For a learned policy-value claim, use an independent holdout or appropriate off-policy evaluation. Compare with the institutional status quo, best uniform policy, or other relevant comparator as the claim requires; do not treat fitted-sample structural counterfactuals as held-out policy rewards.
6. If a claim cannot be supported, weaken it in the Abstract and Introduction first; those are the two places reviewers punish overclaiming.
7. Keep the stakes concrete: name what is acquired, earned, or lost (customers who pay and customers who generate informative data; revenue, not "performance").

## Output Contract

When asked to draft or rewrite, return:

1. A compact outline (3–7 bullets) organized by research question, not by section boilerplate.
2. Revised paragraphs, with useful role labels such as `context / debate / question / challenge / approach / prediction / finding / mechanism / policy / implication` when requested.
3. A claim map for every major claim:
   `Claim: … | Support: appropriate estimate / evaluation / sourced fact / documented case / proof / suggestive descriptive / implementation argument | Baseline: comparator or context, if applicable | Status: supported / suggestive / needs evidence / overclaimed`
4. A short self-review: clarity, nearby economic explanation, identification gaps, and whether any policy-value claim rests only on fitted-sample evidence.
