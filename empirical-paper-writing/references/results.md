# Results Writing Guide (Empirical Papers)

## The Fixed Order

Report findings as average effect → mechanism → heterogeneity → policy value. This is the order of the argument, not the order the analyses were run. Each stage gets one short section.

## Average Effect

1. Use the simplest credible estimator first: means under randomization, defended as best practice.
2. Summarize randomization and balance checks in one paragraph, with appendix pointers.
3. Flag the surprise. State the direction theory predicts, then the result, then promise the explanation ("Section 5 explains why").

## Mechanism

1. Build a discriminating scorecard: one theory ruled out, one supported, optionally one novel behavioral trace. "We explore mechanisms" is not a scorecard.
2. Where two opposing forces are at work, draw them in a diagram.
3. Correlation with a mediator is not a mechanism. Where a link is non-causal, say so (a footnote disclaimer is enough).
4. Rebut the strongest rival story explicitly, in its own paragraph.

## Heterogeneity

1. Interpret substantively: who benefits, which segments, stated as a rule a manager could use.
2. Never dump subgroup tables. Each reported split must change what an actor would do.
3. Use heterogeneity as the bridge that licenses personalization: if effects do not vary in an actionable way, a policy section is not earned.

## Policy Value

1. Introduce the formal policy setup only after the reduced-form evidence earns it.
2. State the policy space and why brute force fails (the number of possible assignments explodes with covariates).
3. Evaluate by an out-of-sample or bias-corrected off-policy estimator (such as inverse propensity scoring). In-sample policy value is not reportable.
4. Compare against both the institutionally real status quo and the best uniform policy, and test the personalized-versus-uniform gap for significance.
5. Own modest gains and give a mechanical reason (little heterogeneity to exploit, small segments).
6. Where long-run outcomes exist, report them and explain which short-run measures act as surrogates; say what is lost when policies are optimized on the short run.

## Negative Results and Robustness

1. A failing rival method is a finding, not a footnote. Name it, show it, diagnose why (too little heterogeneity found, or spurious heterogeneity fit). This is the cautionary co-headline pattern.
2. Tier robustness: one paragraph plus appendix pointers. Footnotes absorb caveats.
3. Show train and test side by side; the test result is authoritative.

## Style

1. Every gain is a percentage with a named baseline in the same sentence.
2. Put numbers in sentences rather than behind table pointers.
3. A "managers should…" sentence may close each results subsection.
4. Repeat headline numbers verbatim wherever they appear (abstract, introduction, results, conclusion).

## Checklist

1. Do findings appear in the fixed order, regardless of analysis chronology?
2. Is the average effect the simplest credible estimator, with the surprise flagged?
3. Does the mechanism section hold a discriminating scorecard and a rebuttal of the strongest rival?
4. Is every heterogeneity result interpreted as an actionable rule?
5. Is policy value out-of-sample or off-policy estimated, against the status quo and the best uniform policy?
6. Is any failing rival method reported and diagnosed?
7. Does every gain carry a number, a named baseline, and a test or interval?
8. Are headline numbers identical across abstract, introduction, results, and conclusion?
