# Introduction Writing Guide (Method Papers)

## Goal

The introduction must earn the puzzle, the failure, and the design. By its end the reader should believe that the problem is real, that existing tools fail at it in a demonstrated way, and that the proposed tool is the natural answer.

## Backward Reasoning First

1. What pattern or decision problem does the paper start from?
2. What do existing tools produce instead, and how will you demonstrate it?
3. What are the primitives of the tool, and what do they make computable?
4. Which track arc do the results follow (theory, structural, ML)?
5. What does an actor now choose or do?
6. Which two literatures does the paper address, and what can neither do alone?
7. What is the one-sentence version of the diagnosis?

## Section Skeleton

```latex
\section{Introduction}
% 1. Context / puzzle: the dichotomy, the institution and friction, or the incumbent practices
% 2. Diagnosis: why existing approaches fail, with evidence
% 3. Our approach: primitives and components, mapped to the named failures
% 4. Findings (with numbers) and contributions by audience
% Roadmap: optional
```

## Opening Moves (choose one)

1. **Anecdote dichotomy (theory).** Matched real-world cases on both sides of the behavior, then an explicit escalating list of research questions.
2. **Institution plus friction (structural).** Define the unfamiliar market, document its stakes, name the economic friction, and state the gap explicitly.
3. **Incumbent-practice taxonomy (ML).** The two ways practitioners now solve the task, each with its virtue and its named failure mode; the method will inherit both virtues.

## The Diagnosis Paragraphs

The signature of method introductions: the failure is demonstrated in the introduction itself.

1. Quantified mispredictions from the paper's own inferior models, a motivating data figure, or the measured performance of the pure approaches.
2. Challenges are stated before the approach, so the design arrives as the answer to a named problem.

## The Approach Paragraphs

1. Name the primitives. The reader leaves knowing what object is built or estimated and what it makes computable.
2. Map each component to the failure it addresses.
3. For borrowed standard parts, give one clause of description and spend the words on why each is the right tool.

## Findings Preview and Contributions

1. A full preview with numbers is the genre norm. Order follows the track arc.
2. Label contributions by audience (methodological, substantive, managerial, policy). Each ends with "Unlike the closest work, we…". See `examples/contribution-statement-template.md`.
3. The roadmap is optional and is often omitted.

## Anti-Patterns

1. Opening with the literature.
2. Opening with the method before the problem exists.
3. A challenge list that is a complaint about prior accuracy.
4. Findings in the order the analyses were run.
5. Contributions that restate findings.
6. A paragraph whose first sentence does not state its message.
7. Opening with "recent advances in [technology]".
8. Presenting the method as an improvement over a naive version of itself.
9. Hiding the absence of formal guarantees. State it and give limiting cases instead.

## Checklist

1. Could a reader who stops after the diagnosis state what fails and why?
2. Does every component map to a named failure?
3. Does the findings preview follow the track arc, with numbers and baselines?
4. Is each contribution stated as a capability, with an "Unlike…" contrast?
5. Reverse outline: thesis → topic sentences → evidence. Is anything unmapped?
