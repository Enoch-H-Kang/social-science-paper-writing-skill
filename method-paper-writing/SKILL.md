---
name: method-paper-writing
description: Write and revise theory, structural, and ML-method papers aimed at quantitative marketing and management journals. Establish the question or obstacle, explain the method and its economic meaning, use validation appropriate to the claim, and benchmark comparative gains when made. Use when drafting or revising the Abstract, Introduction, Literature, Model/Framework, Results/Validation, or Conclusion, or for a pre-submission review. Triggers: "write a method paper", "revise my model section", "method paper 써줘", "이론 논문 고쳐줘", "구조모형 논문 다듬어줘", "Marketing Science 스타일로 모델 논문 써줘".
---

# Method Paper Writing

Adapted from an MIT-licensed research-paper-writing package. The target is a paper whose principal contribution develops a tool. The sampled venues are Management Science and Marketing Science plus one manuscript; other journals in the description are target venues, not sampled style evidence. Reverse outlines, claim maps, role labels, prose quotas, review loops, and LaTeX assembly checks are general editorial aids, not documented drafting practice in the sampled papers.

## Which skill should I use?

Classify by the question and hierarchy of contributions across the abstract and introduction. A tool developed as the main contribution favors this skill; a market or policy answer favors `empirical-paper-writing`. A model or framework named in an abstract does not alone determine the primary route.

Hybrid papers use both skills and the primary one follows the headline.

- Headline is the tool and the market answer is its payoff (a structural framework whose counterfactuals price a market feature; an ML method whose evaluation embeds a managerial finding): this skill is primary, and the empirical skill governs the data and validation sections.
- Headline is a market answer delivered through method components: the empirical skill is primary, and this skill governs the component sections.

This skill works on its own. If the sibling is not installed, apply the rules here and say so when the paper's core is an empirical answer.

## The Three Tracks

Every guide in this skill distinguishes the tracks where they differ. Identify your track before loading any guide.

- **Theory.** An analytical or game-theoretic model. The observed dichotomy is the sampled route; delegation and capability routes are unverified extrapolations.
- **Structural.** An estimation framework built on an explicit model of agent decisions. Typical headline: a framework that corrects a named bias, with counterfactuals that convert estimates into money or guidelines.
- **ML-method.** An algorithm or learning framework. Typical headline: a hybrid that beats the pure approaches and the status-quo practice, with the gain located by regime.

## The One-Sentence Test

Before any sentence-level edit, the paper must pass this test in one breath:

> What [pattern, decision, or capability] matters, and what [question or obstacle] remains? What [model, framework, or algorithm] and [key primitive] address it? Which [formal result, fit, benchmark, or evaluation] supports the claim, under what conditions? What [result, enabled task, caution, or implication] follows?

Use the prompts that apply to the paper. If a necessary answer is missing, fix the argument before polishing prose.

## Core Workflow

1. **Question first.** Establish the question or obstacle before the solution appears; preview a later demonstration truthfully when needed.
2. **Primitives and nearby economic explanation.** The reader should be able to retell the model or method in words, whether interpretation precedes or follows a formal statement.
3. **Load only the section guide you need** (list below). Do not load all references at once.
4. **Rewrite paragraph by paragraph.** Keep a coherent purpose; cases or formal objects can precede the lesson they establish.
5. **Reverse-outline each section** after drafting: thesis → paragraph topic sentences → evidence under each.
6. **Run the claim map** (Output Contract). Match claims to analytical proofs, estimates and model checks, benchmarks, sourced institutional facts, documented cases, explicitly suggestive descriptives, or implementation arguments at their stated strength.
7. **Run the adversarial review** in `references/paper-review.md` and revise until no high-risk item is open.

Use a brief reader-facing dependency explanation when the relationship among components would otherwise be difficult to follow. A topic sentence or ordinary roadmap can suffice. At a consequential transition, connect a completed finding to the next question if that connection helps; a section may instead end on its finding, interpretation, limitation, or implementation pointer.

## The Ten Rules

1. **Start from the practice, dichotomy, or measured obstacle the tool serves.** A market pattern, managerial need, or documented failure of an existing method can establish the question.
2. **Name the actors, objectives, and relevant constraint or tension.** Describe conflicting incentives when the paper has them; a resource limit or open capability question can also motivate the tool.
3. **State the motivating question plainly.** A two-sided tradeoff fits an explanatory dichotomy; a delegation or capability paper may ask a different question.
4. **Question or obstacle before design.** Establish it with observed cases, measured rival failure, an identification gap, infeasibility, or a labeled construction. Keep the evidentiary limit clear.
5. **Results follow a track-appropriate arc.** The theory, structural, and ML outlines below are source-shaped options; choose the order and checks that answer the paper's claims.
6. **Quantify comparative gains when claimed.** Name the baseline and relevant regime; state where the gain vanishes when that is part of the result.
7. **End on the strongest supported result, payoff, caution, boundary, or implication.** Attach decisive conditions to the claims they bound.
8. **Keep intelligible economic explanation near formalism.** A definition or proposition can come first, followed by its interpretation and practical perspective where supported.
9. **Crisp is a quality standard.** Short declarative sentences, one finding per sentence, numbers in sentences, terms defined by what an actor does before notation. Cut any sentence a reader must parse twice.
10. **Defend consequential modeling choices.** Use required properties, tractability, institutional fit, or a business constraint. For an explanatory dichotomy, the model must generate both sides of the phenomenon. For other formal results, check that the statement answers the actual question under its assumptions.

## Method paper choices

| Question or evidence | Useful presentation choice |
|---|---|
| Explanatory theory | Cases or setup → result → nearby interpretation; a benchmark may clarify the main result |
| Structural framework | Decisions and identification → estimates → fitted-sample model checks → counterfactuals, with assumptions explicit |
| ML method | Measured incumbent diagnosis → hybrid design → relevant benchmarks and boundaries |
| Comparative gain | Relevant comparator and regime; tuning and runtime when they affect the claim |
| Formal capability | Precise theorem and conditions; limiting cases can inform claims without invented guarantees |
| Conclusion | Supported payoff, scope, or concrete future question |

Keep terminology stable and weaken claims that exceed the evidence.

## Section Guides

Load only the needed file from `references/`:

- Abstract (three tracks, with optional theory routes): `references/abstract.md`
- Introduction: `references/introduction.md`
- Literature and positioning: `references/literature-and-positioning.md`
- Model and framework (core guide, three tracks): `references/model-and-framework.md`
- Results and validation (including an adapted capability-results route for theory): `references/results-and-validation.md`
- Conclusion: `references/conclusion.md`
- Pre-submission review: `references/paper-review.md`
- Style evidence base: `references/style-evidence.md`
- Fill-in templates (theory has independent dichotomy, delegation, and optional capability routes): `references/examples/abstract-template-theory.md`, `references/examples/abstract-template-structural.md`, `references/examples/abstract-template-ml-method.md`, `references/examples/proposition-intuition-template.md`, `references/examples/contribution-statement-template.md`

## Execution Rules

1. Identify the track before drafting.
2. For each component or proposition, write one line: which question or obstacle it addresses, which primitive it builds, and which counterfactual, characterization, or capability it makes available.
3. Measured failures of restricted or naive versions can motivate a design; state the comparison and its scope.
4. When making comparative performance claims, keep the benchmark protocol fair and disclosed, with tuned rivals and a relevant status-quo practice when applicable.
5. Handle anomalies honestly: surface and resolve oddities, never bury them.
6. Weaken unsupported claims in the abstract and introduction first.
7. Keep notation stable: one symbol, one object, everywhere.

## Output Contract

When asked to draft or rewrite, return:

1. A compact outline (3–7 bullets) organized by question or proposition.
2. Revised paragraphs, with useful role labels such as `context / diagnosis / setup / intuition / formal / comparative-static / validation / benchmark / implication` when requested.
3. A claim map for every major claim:
   `Claim: … | Support: proof / estimate and model check / benchmark / sourced fact / case / suggestive descriptive / implementation argument | Baseline: comparator or not applicable — reason | Status: supported / suggestive / needs evidence / overclaimed`
4. A short self-review: clarity, nearby economic explanation, material assumptions, and comparative gains whose regime or comparator is unclear.
