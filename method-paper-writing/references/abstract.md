# Abstract Writing Guide (Method Papers)

## Goal

A method abstract compresses the argument: the observed pattern, decision problem, or capability sought; the question or obstacle; the offer and its primitive in plain words; and the supported result. The track versions are starting points, not sentence obligations. End on the strongest supported result, payoff, caution, boundary, or implication.

**Compress motivation before the contribution.** Once the task and obstacle are clear, move to what the paper does. Keep an extended hypothetical failure story in the introduction; use the abstract's remaining space for the construction, findings, and their mechanism. Distinguish motivating possibilities from diagnostic results established by the paper.

## Pre-Writing Questions

1. What question or obstacle motivates the tool? If an existing approach fails, what evidence establishes that failure?
2. What is the key primitive your tool builds?
3. What does the primitive make computable or possible (a characterization, a counterfactual, a decision rule, or a capability)?
4. Which track arc do the results follow?
5. What result, payoff, caution, boundary, or implication best closes the abstract?

If questions 1 and 5 have no answer, the abstract is a promise, not a summary.

## Version T: Theory — Explain a Dichotomy, Price Delegation, or Enable a Capability

**Source and variation.** The dichotomy slots follow the theory exemplar's information-choice and taste-signaling arc. Conditional results and economic interpretation recur across analytical components in the corpus. Delegation and capability are unverified extrapolations, and the slot counts are editorial adaptations.

Choose the route that fits the formal question. The first route has nine slots plus Slot 4b:

1. **Observed dichotomy:** "There exists a dichotomy in the [strategies / practices] of [actors in market]—some [actors] [action 1], whereas others [action 2]."
2. **Existing models cannot explain it:** "This divide in [strategies] cannot be explained by existing [benchmark] models."
3. **The offer:** "We offer a model of [phenomenon]." Keep the phenomenon broad; do not narrow it to a tactical variable or add track adjectives such as "analytical."
4. **Modeling premise in plain words:** the dual role or the two forces built in.
4b. **Dilemma:** "In this context, we show that [actor] faces a dilemma—if it [action 1], then [intermediate agent response]."
5. **Tradeoff, first half, as a standalone deduction:** "[Action 1] thus preserves [X] but reduces [Y]."
6. **Tradeoff, second half,** as a mirrored sentence: action 2 undermines [X] but increases [Y]. Keep the pair parallel in structure.
7. **Conditions derived** under which each action occurs.
8. **Emergence bonus** when established: in the dichotomy exemplar, the most tasteful product becomes the hit; a welfare result would be a separate adaptation requiring proof.
9. **Optional implication** for an actor, without notation.

**Optional delegation route (unverified extrapolation):** The source corpus has no delegation abstract or shortcut-pricing model. Begin with the decision an actor cannot fully specify, identify the delegate's possible shortcut, state the open pricing or mechanism-design question, introduce the mechanism and its decisive property, then give the formal result and its conditions. Add an actor implication only when the result supports one. This route does not require two observed actions or an emergence result.

**Optional capability/enabling route (theorem adaptation is an extrapolation):** The source corpus shows enabling-method rhetoric, but no sufficiency or equivalence abstract template. Use this seven-slot sequence when the paper's actual theorem is about what a construction makes possible:

1. **Task or capability sought:** what an actor or analyst wants to accomplish.
2. **Open feasibility or adequacy question:** what remains unestablished for the identified setting or comparator. Claim a demonstrated failure only when one exists.
3. **Setup and enabling property:** relevant information, resources, or procedure and the property that makes the construction work, in plain words.
4. **Main formal result:** what is sufficient, necessary, or equivalent, and for which outcome. Do not turn sufficiency into equivalence or an asymptotic result into a finite-resource claim.
5. **Reason or intuition:** why the property yields the result; merge this with slot 3 when clearer.
6. **Scope or boundary:** attach decisive conditions to the setup or result they bound; use a separate sentence only if it adds information.
7. **Optional closing payoff:** an enabled task, theoretical consequence, practical implication, or unresolved boundary supported by the paper.

Merge slots when the argument reads more clearly that way. This route requires no opposing actions, mirrored tradeoff, numerical superiority, welfare bonus, or failed incumbent.

Template: `examples/abstract-template-theory.md`.

## Version S: Structural — Estimate and Counterfact

**Source and variation.** The institution, dynamic decision, selection, valuation sequence follows the structural exemplar. Conditional claims and counterfactual interpretation recur in method papers. Exact slot counts, numeric bias, and a dollar payoff in the abstract are adaptations rather than observed requirements.

Ten slots:

1. **Setting** defined in a clause.
2. **Friction** (information asymmetry, search cost, uncertainty about quality).
3. **Debated remedy or open question.**
4. **Contribution = the framework.**
5. **The agent's per-period decision** (one sentence).
6. **Its tradeoffs** (one sentence).
7. **The bias hook:** explain when ignoring [dynamics / selection] can bias [parameter] and give a direction only under conditions that support it.
8. **Data** in one clause, with scale only if useful.
9. **Findings:** forward-looking behavior, the substantive finding that buyers value reputation in the structural exemplar, and diagnostic bias at their supported strengths.
10. **Counterfactual payoff or promise:** a valuation exercise and intended managerial use may be stated without an abstract dollar amount; qualify conditional inference.

Template: `examples/abstract-template-structural.md`.

## Version M: ML Method — Diagnose and Hybridize

**Source and variation.** The diagnosis of tested pure approaches followed by a hybrid method follows the ML-method exemplar. Question-first motivation and qualified results recur across method papers. A strict ranking or deployment note in the abstract is an optional adaptation.

Eight slots:

1. **Managerial need.**
2. **Data and evaluation of the pure approaches** on a large real archive.
3. **Diagnostic negative result:** which tested pure approaches fall short, with a ranking only when useful and supported.
4. **One-line verdict,** the empirical contribution in one sentence.
5. **Method announcement:** the named framework.
6. **Mechanism in one line:** how it addresses the tested approaches' limitations.
7. **Result versus named baselines tested,** including the status-quo practice when evaluated; identify the regime where the advantage is supported.
8. **Scope or generalizability close,** if supported; a result or caution may close instead.

Template: `examples/abstract-template-ml-method.md`.

## Scope Placement

Name the setting early. Attach decisive conditions to the claims they bound, state model assumptions where the setup needs them, and gather broader limitations later. A framework may transfer to another setting even when a particular finding does not; state the requirements for each separately.

## Sentence-Level Rules

1. Verbs do the work: *we use, we find, we show, we offer, we develop, we evaluate, we derive*. No "leverages", "sheds light on", "delves into". Use first-person possessives for the contributed method and final takeaways ("our framework," "our machine learning framework," "our results"), but leave standard analytical exercises unpossessed ("Theoretical and empirical counterfactuals show"). Do not stack reporting clauses in consecutive sentences ("We find that..." then "We further show that..."); let the phenomenon lead the follow-on decomposition ("These gains mainly stem from...").
2. Keep multi-finding sentences intelligible; split them when their logic becomes hard to follow.
3. State the comparator for a quantitative gain in the sentence or clear nearby context.
4. No citations, no notation, no undefined acronyms.
5. About 200 words is the ceiling; keep the findings and the strongest supported close.
6. "Novel" appears at most once, attached to the framework.
7. State quantitative gains by regime when the result makes such a comparison.
8. Repeat the tool's name when it aids clarity.
9. No theorem numbers in the abstract.
10. When a regime label is an ordinary English verb or noun, such as `cloak` or `flaunt`, use it directly as a verb on first mention, without a parenthetical or quotation-mark gloss.

## Checklist

1. Does the chosen route fit the paper's actual question and result? Borrow a useful slot from another route when it improves that fit.
2. Is the motivating question or obstacle established at the strength the evidence warrants?
3. Are the primitive and its payoff named?
4. Does the close state the strongest supported result, payoff, caution, boundary, or implication? Are decisive conditions attached to the claims they bound, wherever those claims appear?
