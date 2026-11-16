# Literature and Positioning Guide (Empirical Papers)

In this field the literature section is usually woven into the Introduction or kept short and separate. Either way its job is positioning, not coverage.

## Goal

Place the paper at the intersection of two or three literatures, at least one substantive (the market phenomenon) and at least one methodological (the estimation or design approach). Make the gap a question none of them can answer, not a technique none of them used.

## Workflow

1. List the literatures, not the papers: for example (i) the economics of privacy and targeting, (ii) ML for personalization, (iii) auction and market design. Two or three, never five.
2. Write one paragraph (or one compact block in the introduction) per literature with the template below.
3. Close with the positioning sentence: what this paper does that requires combining what the literatures keep separate.

## Paragraph Template (per literature)

1. Topic sentence naming the literature by its question: "A first stream of work asks how much targeting information is worth to advertisers."
2. What the stream established, in two or three findings attributed to the two or three papers a reviewer would insist on. State what is now known, not paper summaries.
3. What the stream assumes away or cannot compute: no equilibrium, no counterfactual policies, observational data without variation, prediction without incentives.
4. Transition: the missing piece is exactly one of this paper's challenges (name it, linking back to the introduction).

## Rules

1. **Position against questions, not against papers.** Never write a sequence of "X (Year) did A. However, they did not do B." That reads as a takedown list.
2. **The closest paper gets the most respectful and most precise treatment.** State its contribution in terms its author would accept, then the one dimension on which this paper differs, and make the difference a question ("they estimate the value of targeting under the observed regime; we ask what happens to each player's payoff under counterfactual regimes"), not a resource ("we have more data").
3. **Cite the canonical version.** Journal version over working paper when one exists.
4. **No citation dumps.** A sentence with more than three citations is doing taxonomy, not argument; split or cut it.
5. **Cite method literatures for capability and for known failure modes.** When borrowing an estimator, cite its source and the paper that characterizes when it fails in settings like yours; this pre-answers the methods reviewer.
6. **End each stream's paragraph with what the stream cannot answer,** phrased as one of the paper's challenges.
7. **One stream may be cautionary.** Prior work showing the naive version of your own approach failing (personalization that does not beat a uniform rule, say) pre-answers the methods reviewer and motivates your design.

## Checklist

1. Two or three literatures, each ending in a gap that names one of the paper's challenges?
2. Closest work treated precisely and respectfully, with the difference stated as a question?
3. Every claim about prior findings traceable to the cited paper's actual result?
4. Does the closing positioning sentence require the combination of components rather than either alone?
5. Is one stream, where relevant, used cautionary to pre-answer the methods reviewer?
