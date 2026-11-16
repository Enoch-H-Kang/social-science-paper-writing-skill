# Paper Writing Skills for INFORMS-Style Journals

Two self-contained agent skills for writing and revising quantitative marketing, information systems, and management papers, aimed at journals such as Management Science, Marketing Science, the Journal of Marketing Research, Information Systems Research, and Quantitative Marketing and Economics. The guidance is distilled from the section structure, abstract formulas, and results rhetoric of published papers in those journals, and it is adapted from an ML-conference writing skill package (credited below). Each skill teaches an agent how to draft, restructure, and adversarially review a paper section by section.

## The two skills

- **`empirical-paper-writing/`** is for papers whose contribution is an *answer about a market*: field and natural experiments, causal analyses of platform or firm data, and policy or design evaluations. Its core guide covers data and identification. Results follow a fixed order: average effect, mechanism, heterogeneity, policy value.
- **`method-paper-writing/`** is for papers whose contribution is a *tool*: analytical or game-theoretic models, structural estimation frameworks, and ML or econometric methods. The three tracks are kept separate in every guide that differs by track (abstract, model/framework, results and validation).

## Which skill should I use?

Classify the paper by where the headline contribution claim sits, that is, the contribution sentence of the abstract. If it promises a market or policy answer, use the empirical skill. If it promises a tool (a model, framework, estimator, or algorithm), use the method skill.

Hybrid papers use both skills; the primary skill follows the headline.

- Market answer delivered through method components: the empirical skill is primary and the method skill governs the component sections.
- Tool is the headline and the market answer is its payoff: the method skill is primary and the empirical skill governs the data and validation sections.

| Archetype | Primary skill |
|---|---|
| Randomized field experiment ending in a personalized policy | Empirical |
| Game-theoretic model explaining an observed dichotomy | Method (theory track) |
| Dynamic structural framework whose counterfactuals price a market feature | Method (structural track), empirical secondary |
| ML measurement feeding an economic model to answer a policy question | Empirical primary, method secondary |

## Install / use

Copy a skill folder into your agent's skills directory (for example `~/.claude/skills/` for Claude Code), or point an OpenAI-style agent at the skill's `agents/openai.yaml`. Each skill is self-contained: install only the one you need. Each `SKILL.md` is the only file loaded by default and tells the agent which section guide to load for the task at hand.

## Layout

```
empirical-paper-writing/
  SKILL.md, agents/openai.yaml
  references/
    abstract.md  introduction.md  literature-and-positioning.md
    data-and-identification.md  results.md  conclusion.md
    paper-review.md  style-evidence.md
    examples/  abstract-templates.md  introduction-question-set-template.md
               contribution-statement-template.md
method-paper-writing/
  SKILL.md, agents/openai.yaml
  references/
    abstract.md  introduction.md  literature-and-positioning.md
    model-and-framework.md  results-and-validation.md  conclusion.md
    paper-review.md  style-evidence.md
    examples/  abstract-template-theory.md  abstract-template-structural.md
               abstract-template-ml-method.md  proposition-intuition-template.md
               contribution-statement-template.md
```

## How these differ from ML-conference writing

ML-conference writing opens with a technical challenge, sells a pipeline figure, and proves itself by beating baselines. Journal writing in this tradition opens with a market practice and a tension between named actors, poses numbered research questions, treats identification or validation as main-text obligations, and closes on what an actor will now do. Each `SKILL.md` contains a short contrast table making these differences explicit.

## Attribution and license

Released under the MIT License. These skills adapt [Master-cai/Research-Paper-Writing-Skills](https://github.com/Master-cai/Research-Paper-Writing-Skills), which packages Prof. Peng Sida's paper-writing notes. What was kept from that package is its workflow discipline: one paragraph, one message; reverse outlining; claim-evidence maps; adversarial self-review. What was replaced is all of the substance, retargeted from ML conferences to INFORMS-style journals. See `LICENSE` for the full text.
