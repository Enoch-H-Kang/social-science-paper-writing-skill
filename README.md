# Paper Writing Skills for INFORMS-Style Journals

Two self-contained agent skills for writing and revising quantitative marketing, information systems, and management papers, aimed at journals such as Management Science, Marketing Science, the Journal of Marketing Research, Information Systems Research, and Quantitative Marketing and Economics. The sampled papers come from the first two journals and one manuscript; the other journals are targets, not sources of sampled style evidence. The guides adapt observed section structures and rhetoric alongside general editorial advice. Each skill teaches an agent how to draft, restructure, and review a paper section by section.

## The two skills

- **`empirical-paper-writing/`** is for papers whose contribution is an *answer about a market*: field and natural experiments, causal analyses of platform or firm data, and policy or design evaluations. Its core guide covers data and identification. Results can follow the field-experiment arc (average effects, mechanisms, policy design/value, a return to segmentation and mechanism, then long-run outcomes) or the targeting hybrid arc (prediction, targeting value, analytical model, then market counterfactuals).
- **`method-paper-writing/`** is for papers whose contribution is a *tool*: analytical or game-theoretic models, structural estimation frameworks, and ML or econometric methods. The three tracks are kept separate in every guide that differs by track (abstract, model/framework, results and validation).

## Which skill should I use?

Classify the paper by its question and hierarchy of contributions across the abstract and introduction. A market or policy answer favors the empirical skill; a tool whose development and general use are the main contribution favors the method skill. A framework named in the abstract does not alone settle the route.

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

## Evidence and editorial approach

The sampled papers show several ways to motivate market questions, explain identification or validation, and close with findings, cautions, implications, or future questions. The guides use these as options rather than venue-wide rules. Reverse outlines, claim maps, role labels, review loops, prose quotas, and LaTeX assembly checks are general editorial aids; the finished papers do not establish their authors' drafting process.

## Attribution and license

Released under the MIT License. These skills adapt an MIT-licensed research-paper-writing package. Reverse outlining, claim-evidence maps, and adversarial self-review remain editorial aids. See `LICENSE` for the full text.
