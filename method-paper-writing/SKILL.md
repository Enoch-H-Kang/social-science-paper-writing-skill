---
name: method-paper-writing
description: Write and revise method papers for INFORMS-style journals (Management Science, Marketing Science, Journal of Marketing Research, Information Systems Research, QME) — analytical/game-theoretic models, structural estimation frameworks, and ML/econometric methods, each handled as its own track. Open with the observed pattern, decision problem, or capability the tool serves; establish the question or obstacle before presenting the solution; give intuition before math; validate claims against the appropriate model, data, or limiting cases; and benchmark comparative performance claims against relevant approaches. Use when drafting or revising the Abstract, Introduction, Literature, Model/Framework, Results/Validation, or Conclusion of a theory, structural, or ML-method paper, or for a pre-submission adversarial review. Triggers: "write a method paper", "revise my model section", "method paper 써줘", "이론 논문 고쳐줘", "구조모형 논문 다듬어줘", "Marketing Science 스타일로 모델 논문 써줘".
---

# Method Paper Writing

Adapted from an MIT-licensed research-paper-writing package. That package teaches ML/CV/NLP conference writing: teaser figure, pipeline, beat SOTA, ablate. This skill keeps its discipline (one paragraph = one message, reverse outlining, claim–evidence checks, adversarial self-review) and replaces its substance. The target is a method paper in the house style of quantitative marketing and management journals: a paper whose contribution is a tool.

## Which skill should I use?

Classify the paper by where the headline contribution claim sits (the contribution sentence of the abstract). A tool (model, framework, estimator, algorithm) means this skill. A market or policy answer means the sibling skill, `empirical-paper-writing`, which covers field and natural experiments, causal analyses of platform or firm data, and policy or design evaluations.

Hybrid papers use both skills and the primary one follows the headline.

- Headline is the tool and the market answer is its payoff (a structural framework whose counterfactuals price a market feature; an ML method whose evaluation embeds a managerial finding): this skill is primary, and the empirical skill governs the data and validation sections.
- Headline is a market answer delivered through method components: the empirical skill is primary, and this skill governs the component sections.

This skill works on its own. If the sibling is not installed, apply the rules here and say so when the paper's core is an empirical answer.

## The Three Tracks

Every guide in this skill distinguishes the tracks where they differ. Identify your track before loading any guide.

- **Theory.** An analytical or game-theoretic model. Possible headlines: an explanation of an observed dichotomy, a delegation mechanism, or a formal result enabling a capability.
- **Structural.** An estimation framework built on an explicit model of agent decisions. Typical headline: a framework that corrects a named bias, with counterfactuals that convert estimates into money or guidelines.
- **ML-method.** An algorithm or learning framework. Typical headline: a hybrid that beats the pure approaches and the status-quo practice, with the gain located by regime.

## The One-Sentence Test

Before any sentence-level edit, the paper must pass this test in one breath:

> What [pattern, decision, or capability] matters, and what [question or obstacle] remains? What [model, framework, or algorithm] and [key primitive] address it? Which [formal result, fit, benchmark, or evaluation] supports the claim, under what conditions? What [result, enabled task, caution, or implication] follows?

Use the prompts that apply to the paper. If a necessary answer is missing, fix the argument before polishing prose.

## Core Workflow

1. **Question first.** Establish the question or obstacle before the solution appears; preview a later demonstration truthfully when needed.
2. **Primitives and intuition before notation.** The reader should be able to retell the model or method in words.
3. **Load only the section guide you need** (list below). Do not load all references at once.
4. **Rewrite paragraph by paragraph.** One message per paragraph; the first sentence states the message.
5. **Reverse-outline each section** after drafting: thesis → paragraph topic sentences → evidence under each.
6. **Run the claim map** (Output Contract). Every claim must point to a proposition, an estimate plus fit, or a benchmarked gain.
7. **Run the adversarial review** in `references/paper-review.md` and revise until no high-risk item is open.

## The Ten Rules

1. **Start from the practice or the dichotomy the tool serves, never from what methods cannot do.** The opening is a plain fact about a market, a pattern in behavior, or a managerial need. Never open with "recent advances in…".
2. **Name the actors, objectives, and relevant constraint or tension.** Describe conflicting incentives when the paper has them; a resource limit or open capability question can also motivate the tool.
3. **State the motivating question plainly.** A two-sided tradeoff fits an explanatory dichotomy; a delegation or capability paper may ask a different question.
4. **Question or obstacle before design.** Establish it with observed cases, measured rival failure, an identification gap, infeasibility, or a labeled construction. Keep the evidentiary limit clear.
5. **Results follow the track arc.** Theory: benchmark → main result → comparative statics → extensions. Structural: estimates against nested inferior models → fit → counterfactuals. ML: top line → pairwise with why → where the gain is largest → ablation.
6. **Quantify comparative gains when claimed.** Name the baseline and relevant regime; state where the gain vanishes when that is part of the result.
7. **End on the strongest supported result, payoff, caution, boundary, or implication.** Attach decisive conditions to the claims they bound.
8. **Intuition before math, always.** State the idea in plain words, then the formal version. Give the technical answer and its practical perspective when one follows; state a manager rule when the result supports one.
9. **Crisp is a quality standard.** Short declarative sentences, one finding per sentence, numbers in sentences, terms defined by what an actor does before notation. Cut any sentence a reader must parse twice.
10. **Defend every modeling choice on the spot.** Use required properties, tractability with the infeasible alternative sketched, or a business constraint. For an explanatory dichotomy, the model must generate both sides of the phenomenon. For other formal results, check that the statement answers the actual question under its assumptions.

## How this differs from ML-conference writing

| ML/CV conference | INFORMS journal |
|---|---|
| Teaser or pipeline figure as first impression | The dichotomy or decision problem as first impression |
| Method = modules with stated advantages | Framework = primitives, each mapped to a named question or obstacle |
| Theorems expected, or no theory at all | Intuition mandatory and proofs deferred; limiting cases can substitute for theorems when you say honestly that guarantees are open |
| Beat-SOTA tables | Status-quo-anchored benchmarks, with the gain located by regime |
| Tutorial scaffolding minimized | Tutorial scaffolding generous, because readers are quantitatively sophisticated but not specialists |
| Cost and runtime hidden or in an appendix | Cost, runtime, and effort reported when material to a claim |
| Conclusion = future-work boilerplate | Conclusion = supported payoff, limitations, and concrete next questions |

Keep from the conference tradition, unchanged: one paragraph, one message; topic sentence first; reverse outlining; stable terminology; weaken any claim the evidence does not support.

## Section Guides

Load only the needed file from `references/`:

- Abstract (three tracks, with optional theory routes): `references/abstract.md`
- Introduction: `references/introduction.md`
- Literature and positioning: `references/literature-and-positioning.md`
- Model and framework (core guide, three tracks): `references/model-and-framework.md`
- Results and validation: `references/results-and-validation.md`
- Conclusion: `references/conclusion.md`
- Pre-submission review: `references/paper-review.md`
- Style evidence base: `references/style-evidence.md`
- Fill-in templates (theory has independent dichotomy, delegation, and optional capability routes): `references/examples/abstract-template-theory.md`, `references/examples/abstract-template-structural.md`, `references/examples/abstract-template-ml-method.md`, `references/examples/proposition-intuition-template.md`, `references/examples/contribution-statement-template.md`

## Execution Rules

1. Identify the track before drafting.
2. For each component or proposition, write one line: which question or obstacle it addresses, which primitive it builds, and which counterfactual, characterization, or capability it makes available.
3. Never present the design as an improvement over a naive version of itself. Present it as the answer to the named question or obstacle.
4. When making comparative performance claims, keep the benchmark protocol fair and disclosed, with tuned rivals and a relevant status-quo practice when applicable.
5. Handle anomalies honestly: surface and resolve oddities, never bury them.
6. Weaken unsupported claims in the abstract and introduction first.
7. Keep notation stable: one symbol, one object, everywhere.

## Output Contract

When asked to draft or rewrite, return:

1. A compact outline (3–7 bullets) organized by question or proposition.
2. Revised paragraphs, each labeled with its role: `context / diagnosis / setup / intuition / formal / comparative-static / validation / benchmark / implication`.
3. A claim map for every major claim:
   `Claim: … | Support: proposition / estimate+fit / benchmarked gain | Baseline: named comparator or not applicable — reason | Status: supported / needs evidence / overclaimed`
4. A short self-review: sentences to split or cut, intuition-before-math check, undefended modeling choices, and any comparative gain not located by its relevant regime.
