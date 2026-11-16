---
name: method-paper-writing
description: Write and revise method papers for INFORMS-style journals (Management Science, Marketing Science, Journal of Marketing Research, Information Systems Research, QME) — analytical/game-theoretic models, structural estimation frameworks, and ML/econometric methods, each handled as its own track. Open with the market dichotomy or decision problem the tool exists for, demonstrate the failure of existing approaches before presenting the design, give intuition before math, name comparative statics economically, validate against untargeted moments or limiting cases before any counterfactual, and benchmark against pure approaches with the gain located where it is largest. Use when drafting or revising the Abstract, Introduction, Literature, Model/Framework, Results/Validation, or Conclusion of a theory, structural, or ML-method paper, or for a pre-submission adversarial review. Triggers: "write a method paper", "revise my model section", "method paper 써줘", "이론 논문 고쳐줘", "구조모형 논문 다듬어줘", "Marketing Science 스타일로 모델 논문 써줘".
---

# Method Paper Writing

Adapted from Master-cai/Research-Paper-Writing-Skills (itself from Prof. Peng Sida's notes, MIT License). That package teaches ML/CV/NLP conference writing: teaser figure, pipeline, beat SOTA, ablate. This skill keeps its discipline (one paragraph = one message, reverse outlining, claim–evidence checks, adversarial self-review) and replaces its substance. The target is a method paper in the house style of quantitative marketing and management journals: a paper whose contribution is a tool.

## Which skill should I use?

Classify the paper by where the headline contribution claim sits (the contribution sentence of the abstract). A tool (model, framework, estimator, algorithm) means this skill. A market or policy answer means the sibling skill, `empirical-paper-writing`, which covers field and natural experiments, causal analyses of platform or firm data, and policy or design evaluations.

Hybrid papers use both skills and the primary one follows the headline.

- Headline is the tool and the market answer is its payoff (a structural framework whose counterfactuals price a market feature; an ML method whose evaluation embeds a managerial finding): this skill is primary, and the empirical skill governs the data and validation sections.
- Headline is a market answer delivered through method components: the empirical skill is primary, and this skill governs the component sections.

This skill works on its own. If the sibling is not installed, apply the rules here and say so when the paper's core is an empirical answer.

## The Three Tracks

Every guide in this skill distinguishes the tracks where they differ. Identify your track before loading any guide.

- **Theory.** An analytical or game-theoretic model. Typical headline: an explanation of an observed dichotomy, with conditions and an emergence or welfare result.
- **Structural.** An estimation framework built on an explicit model of agent decisions. Typical headline: a framework that corrects a named bias, with counterfactuals that convert estimates into money or guidelines.
- **ML-method.** An algorithm or learning framework. Typical headline: a hybrid that beats the pure approaches and the status-quo practice, with the gain located by regime.

## The One-Sentence Test

Before any sentence-level edit, the paper must pass this test in one breath:

> A [decision problem / observed pattern] in a real market cannot be [answered / explained / computed] with existing tools, because [named failure, demonstrated]. We build [model / framework / algorithm] whose key primitive is [object], which makes [counterfactual / characterization] computable. It is validated by [benchmark model / fit vs. nested alternatives / limiting cases + ablations], and the gain is largest exactly where [regime the user cares about]. This implies [what an actor will now choose / can now do].

If any slot is empty, fix the slot, not the prose.

## Core Workflow

1. **Diagnosis first.** Demonstrate the failure of existing approaches before the design appears.
2. **Primitives and intuition before notation.** The reader should be able to retell the model or method in words.
3. **Load only the section guide you need** (list below). Do not load all references at once.
4. **Rewrite paragraph by paragraph.** One message per paragraph; the first sentence states the message.
5. **Reverse-outline each section** after drafting: thesis → paragraph topic sentences → evidence under each.
6. **Run the claim map** (Output Contract). Every claim must point to a proposition, an estimate plus fit, or a benchmarked gain.
7. **Run the adversarial review** in `references/paper-review.md` and revise until no high-risk item is open.

## The Ten Rules

1. **Start from the practice or the dichotomy the tool serves, never from what methods cannot do.** The opening is a plain fact about a market, a pattern in behavior, or a managerial need. Never open with "recent advances in…".
2. **Name the actors and their conflicting incentives.** Firm vs. consumers, platform vs. advertisers, experimenter vs. traffic budget. A paper without a tension between named actors has no story yet.
3. **The puzzle is a tradeoff stated in two nouns,** and for theory papers the title often names it. If you cannot state it in two nouns, the contribution is not sharp.
4. **Diagnosis before design.** The failure of existing approaches is demonstrated (estimated, benchmarked, or proved), never asserted.
5. **Results follow the track arc.** Theory: benchmark → main result → comparative statics → extensions. Structural: estimates against nested inferior models → fit → counterfactuals. ML: top line → pairwise with why → where the gain is largest → ablation.
6. **Every gain is quantified against a named baseline and located.** State the regime where the gain is largest and where it vanishes.
7. **End on what the tool changes for an actor:** an emergence result, a manager question answered, or deployment conditions.
8. **Intuition before math, always.** State the idea in plain words, then the formal version. State each contribution two ways (technical answer, then business perspective) and end in the simple rule a manager can run.
9. **Crisp is a quality standard.** Short declarative sentences, one finding per sentence, numbers in sentences, terms defined by what an actor does before notation. Cut any sentence a reader must parse twice.
10. **Defend every modeling choice on the spot.** Use required properties, tractability with the infeasible alternative sketched, or a business constraint. The model must generate both sides of the phenomenon it explains, not only its favorite regime.

## How this differs from ML-conference writing

| ML/CV conference | INFORMS journal |
|---|---|
| Teaser or pipeline figure as first impression | The dichotomy or decision problem as first impression |
| Method = modules with stated advantages | Framework = primitives, each mapped to a named failure of existing tools |
| Theorems expected, or no theory at all | Intuition mandatory and proofs deferred; limiting cases can substitute for theorems when you say honestly that guarantees are open |
| Beat-SOTA tables | Status-quo-anchored benchmarks, with the gain located by regime |
| Tutorial scaffolding minimized | Tutorial scaffolding generous, because readers are quantitatively sophisticated but not specialists |
| Cost and runtime hidden or in an appendix | Cost, runtime, and effort accounting reported |
| Conclusion = future-work boilerplate | Conclusion = deployment conditions and actor implications |

Keep from the conference tradition, unchanged: one paragraph, one message; topic sentence first; reverse outlining; stable terminology; weaken any claim the evidence does not support.

## Section Guides

Load only the needed file from `references/`:

- Abstract (three versions by track): `references/abstract.md`
- Introduction: `references/introduction.md`
- Literature and positioning: `references/literature-and-positioning.md`
- Model and framework (core guide, three tracks): `references/model-and-framework.md`
- Results and validation: `references/results-and-validation.md`
- Conclusion: `references/conclusion.md`
- Pre-submission review: `references/paper-review.md`
- Style evidence base: `references/style-evidence.md`
- Fill-in templates: `references/examples/abstract-template-theory.md`, `references/examples/abstract-template-structural.md`, `references/examples/abstract-template-ml-method.md`, `references/examples/proposition-intuition-template.md`, `references/examples/contribution-statement-template.md`

## Execution Rules

1. Identify the track before drafting.
2. For each component or proposition, write one line: which question it answers, which failure of existing tools it addresses, which primitive it builds, which counterfactual or characterization it makes available.
3. Never present the design as an improvement over a naive version of itself. Present it as the answer to the named failure.
4. Keep the benchmark protocol fair and disclosed (tuned grids for rivals, the status-quo practice included).
5. Handle anomalies honestly: surface and resolve oddities, never bury them.
6. Weaken unsupported claims in the abstract and introduction first.
7. Keep notation stable: one symbol, one object, everywhere.

## Output Contract

When asked to draft or rewrite, return:

1. A compact outline (3–7 bullets) organized by question or proposition.
2. Revised paragraphs, each labeled with its role: `context / diagnosis / setup / intuition / formal / comparative-static / validation / benchmark / implication`.
3. A claim map for every major claim:
   `Claim: … | Support: proposition / estimate+fit / benchmarked gain | Baseline: … | Status: supported / needs evidence / overclaimed`
4. A short self-review: sentences to split or cut, intuition-before-math check, undefended modeling choices, and any gain not located by regime.
