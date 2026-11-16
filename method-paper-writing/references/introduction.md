# Introduction Writing Guide (Method Papers)

## Goal

The introduction must establish the question or obstacle before the solution. By its end the reader should understand why the task matters, what is not yet known or feasible, and how the proposed tool addresses it. Preview a demonstration that belongs later without implying it has already been shown.

## Backward Reasoning First

1. What pattern or decision problem does the paper start from?
2. What question or obstacle remains, and what evidence establishes it? If a rival fails, how will you demonstrate that?
3. What are the primitives of the tool, and what do they make computable?
4. Which track arc do the results follow (theory, structural, ML)?
5. What result, capability, or decision follows for the relevant actor or analyst?
6. Which literatures does the paper address, and what does each contribute to the question?
7. What is the one-sentence version of the question or obstacle?

## Section Skeleton

**Source and variation.** The opening options come from separate theory, structural, and ML-method exemplars. Question or obstacle before the offered tool recurs across them. The four-step outline, contribution labels, and optional roadmap are editorial adaptations, not one shared paper architecture.

```latex
\section{Introduction}
% 1. Context / puzzle: the dichotomy, the institution and friction, or the incumbent practices
% 2. Question or obstacle: establish it with evidence appropriate to the claim
% 3. Our approach: primitives and components, mapped to the question or obstacle
% 4. Findings (with numbers where relevant) and contributions by audience
% Roadmap: optional
```

## Opening Moves (choose one)

1. **Anecdote dichotomy (theory).** Matched real-world cases on both sides of the behavior, then an explicit escalating list of research questions.
2. **Institution plus friction (structural).** Define the unfamiliar market, document its stakes, name the economic friction, and state the gap explicitly.
3. **Incumbent-practice taxonomy (ML).** Describe tested approaches and their measured strengths or limits; explain what the proposed hybrid actually combines.
4. **Task or capability sought (theory, optional extrapolation).** State what an actor or analyst needs to accomplish, then the open feasibility or adequacy question before the enabling construction.

## The Diagnosis Paragraphs

Establish the question or obstacle before presenting the design. Choose evidence that warrants the claim:

1. **Observed cases:** document the contrasting practice; cases establish that a pattern exists, not its prevalence or cause.
2. **Measured rival failure:** give fitted-model mispredictions or tested-method performance, with the setting and comparison; the conclusion is limited to those rivals and tests.
3. **Missing information or identification:** name the object that available variation cannot identify and the information the proposed approach adds.
4. **Computational infeasibility:** state the relevant state space or operation and why the existing computation is intractable under the paper's setup.
5. **Labeled constructed example:** state the constructed premises before the illustration and whether it shows a possibility, refutes a universal claim, or supplies intuition. One example does not establish prevalence, an average effect, or general superiority. Using a body-style analytical example in an introduction is an extrapolated placement choice; point to the later proof or evaluation.

The introduction may preview a full formal or empirical demonstration that appears later. Name its location and state only what the preview supports.

## The Approach Paragraphs

1. Name the primitives. The reader leaves knowing what object is built or estimated and what it makes computable.
2. Map each component to the question or obstacle it addresses.
3. For borrowed standard parts, give one clause of description and spend the words on why each is the right tool.

## Findings Preview and Contributions

1. Preview the results that answer the paper's question. Give numbers and baselines for quantitative comparisons; order by the headline contribution.
2. Label contributions by audience (methodological, substantive, managerial, policy). Use a closest-work contrast when a source supports the precise difference; it need not close each paragraph. See `examples/contribution-statement-template.md`.
3. The roadmap is optional and is often omitted.
4. **Check an included roadmap against the paper.** Match section references, order, and body-versus-appendix locations to the final manuscript. Include the major intervening steps in a full-paper roadmap; label a selective preview as selective. Recheck the map after moving or adding sections.

## Anti-Patterns

1. Opening with the literature.
2. Opening with the method before the problem exists.
3. An unsupported complaint about prior accuracy; measured failure can motivate the method.
4. Findings ordered without regard to the paper's question or argument.
5. Contributions that repeat findings without explaining why they matter.
6. A paragraph that introduces a case or formal object but never draws its lesson.
7. Opening with "recent advances in [technology]".
8. Presenting an untested naive comparison as established evidence.
9. Hiding the absence of formal guarantees. State it and give limiting cases instead.

## Checklist

1. Could a reader who stops after the diagnosis state the question or obstacle and its evidentiary basis?
2. Does every component map to a named question or obstacle?
3. Does the findings preview answer the question, with numbers and baselines for quantitative comparisons?
4. Is each contribution stated as a capability or substantive answer, with any closest-work contrast supported by a source?
5. Reverse outline: thesis → topic sentences → evidence. Is anything unmapped?

## Scope Placement

Identify the setting before drawing inferences. Put decisive conditions beside the claims they bound, explain material model assumptions with the setup, and gather other limitations later. A transferable framework may support context-dependent findings; distinguish the requirements for applying the framework from the conditions under which a result transfers.
