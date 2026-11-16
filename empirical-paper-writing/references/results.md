# Results Writing Guide (Empirical Papers)

## Choose a Results Arc

**Source and variation.** The field-experiment exemplar moves from average effects and initial mechanisms to policy design/value, then returns to segmentation and an additional mechanism before long-run outcomes. The targeting hybrid moves from prediction and targeting value to an analytical model and market counterfactuals. Both connect evidence to the economic question; the headings below are editorial options, not a required shared sequence.

## Average Effect

1. For randomized average effects, use a credible simple estimator such as treatment means and explain why it applies.
2. Summarize randomization and balance checks with enough detail for the design; use appendix pointers where helpful.
3. Flag a surprising result when present and explain the expectation it reverses; point to the actual later explanation if needed.

## Mechanism

1. Report the evidence available: a tested rival, a supported channel, or an explicitly suggestive behavioral trace. A rejected-rival scorecard is useful only when tests warrant it.
2. Where two opposing forces are at work, draw them in a diagram.
3. A mediator association may inform a mechanism account if clearly marked suggestive and noncausal.
4. Address a rival story when the paper tests one; this can occur after policy results.

## Heterogeneity

1. Interpret substantively: who benefits and how the segments affect explanation or decision, with a manager rule only when supported.
2. Explain what subgroup tables teach about the phenomenon or decision; an actor rule is needed only when claimed.
3. Heterogeneity may explain policy assignments after the policy section, or clarify effects without a policy recommendation.

## Policy Value

1. Open an off-policy evaluation subsection by announcing the empirical evaluation and quantifying gains over benchmark policies; do not re-explain model construction from an earlier subsection. Assign compact symbolic handles (for example, $\pi_{\text{lasso}}$, $\pi_{30}$) and define each as a formal treatment-prescription rule mapping covariates to a treatment.
2. State the policy space and why brute force fails (the number of possible assignments explodes with covariates).
3. For a learned treatment policy's value, use an independent holdout or suitable off-policy estimator (such as inverse propensity scoring). For inverse propensity scoring, explain propensity scaling and the pseudo-population intuition, then immediately give the formal estimator and define its notation: "Formally, $\widehat R_{\mathrm{IPS}}(\pi)=n^{-1}\sum_{i=1}^{n}\mathbf 1\{A_i=\pi(X_i)\}Y_i/e_i(A_i\mid X_i)$," where $X_i$ are covariates, $A_i$ assigned treatment, $Y_i$ observed reward, $e_i$ assignment propensity, and $\pi$ the proposed policy. Preserve counterfactual modality: "expected rewards," "proposed policy," "if we were to implement," and "we see that." Fitted-sample structural model checks support a different claim.
4. Compare with the relevant institutional status quo, then the best uniform policy when it is a meaningful alternative; test a personalized-versus-uniform gap when claiming it. Without a redundant umbrella topic sentence, signpost the hierarchy: "The key finding is that..." for the status-quo baseline, then "Furthermore, we see that..." for the best uniform benchmark.
5. Own modest gains and give a mechanical reason (little heterogeneity to exploit, small segments). When segmentation has its own subsection, leave treatment-assignment segment shares out of the reward comparison and stop after stating best-uniform dominance; reserve the segment shares and their synthesis for segmentation.
6. Where long-run outcomes exist, report them and explain which short-run measures act as surrogates; say what is lost when policies are optimized on the short run.

## Negative Results and Robustness

1. A failing rival method is a finding, not a footnote. Name it, show it, diagnose why (too little heterogeneity found, or spurious heterogeneity fit). This is the cautionary co-headline pattern.
2. Give material robustness checks the space they need; use appendix pointers for supporting detail.
3. Show train and test results when a generalization or learned-policy claim depends on the split; label fitted-sample structural checks accurately.

## Style

1. Give a comparator for quantitative gains, either locally or through clear nearby context; absolute quantities need no gain baseline.
2. Open a results block by pointing to the relevant table or panel and equating theoretical estimator targets with empirical outcome metrics (for example, "We present the expected rewards (or subscription rates)... in the top panel of Table 8"). Still state headline gains directly in prose, with numbers in sentences rather than behind table pointers.
3. A "managers should…" sentence may close each results subsection.
4. Keep headline numbers substantively consistent across sections; compatible rounding and contextual baselines are acceptable.

## Checklist

1. Does the chosen field-experiment or targeting-hybrid arc fit the question, including any post-policy mechanism return?
2. Is the average effect the simplest credible estimator, with the surprise flagged?
3. Are identified, suggestive, opposing-channel, and tested-rival mechanism claims distinguished?
4. Is heterogeneity interpreted at the strength supported, without an invented actor rule?
5. Is learned-policy value independently evaluated, with comparators relevant to the claim?
6. Is any failing rival method reported and diagnosed?
7. Do quantitative gain claims carry a number and a recoverable comparator, with uncertainty where needed?
8. Are headline numbers substantively consistent under compatible rounding?
