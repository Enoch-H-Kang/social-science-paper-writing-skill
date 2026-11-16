# Results and Validation Guide (Method Papers)

## Principle

Results follow the track arc. Each result gets a *why* paragraph, not just a number. Validation precedes any counterfactual or claim built on the tool.

## Theory Arc

1. **Benchmark model result:** what happens without the key force. This is the default the main result deviates from.
2. **Main proposition,** with a formal statement and a plain-words restatement adjacent to it. Proof deferred. Follow it with interpretation paragraphs tying it to real behavior.
3. **Comparative statics with economic names:** parameter, direction, and the force that drives it, never bare monotonicity. One managerial interpretation each; flag counterintuitive ones.
4. **Dichotomy check:** both observed regimes arise in different parameter regions.
5. **Extensions,** each with its own proposition. Irrelevance results are results.
6. **Every research question** from the introduction is answered by a numbered result.

## Structural Arc

1. **First-stage estimates** briefly; details to the appendix.
2. **Structural parameters against nested inferior models** (static, fewer types), so the bias claim is demonstrated in one table.
3. **An economic story for every coefficient,** tied to the vocabulary of the introduction.
4. **Fit and validation** against untargeted or held-out moments for all competing models, before any counterfactual.
5. **Within-regime simulations** that monetize the estimates.
6. **Regime-change counterfactuals** framed as plain-language manager questions. Each pairs a (possibly surprising) result with its mechanism and a recommendation. State partial-equilibrium caveats, and recast estimates as bounds where honest.

## ML-Method Arc

1. **Top-line claim:** best on average across regimes, shown as a figure plus a pairwise table with significance.
2. **Versus each pure approach,** with the mechanism of the gain explained and its trajectory across regimes (horizon, traffic, sample size).
3. **Where the gain is largest,** aligned with the regime the manager cares about.
4. **The embedded managerial finding:** the status-quo practice is dominated.
5. **Ablations** confirming the design intuition: removing a component should hurt exactly where the intuition says.
6. **Cost and runtime accounting.**
7. **Honest negatives:** regimes without a significant gain are reported as such.

## Shared Rules

1. Every gain: a number, a named baseline, and a stated regime in one sentence.
2. Repeat headline numbers verbatim across abstract, introduction, results, and conclusion.
3. Cross-check one headline result with an independent (for example model-free) method when possible.
4. Surface and resolve anomalies; never bury them.

## Checklist

1. Does the results section follow the arc of the paper's track?
2. Does each result carry a why paragraph?
3. Is validation (fit, benchmark, limiting case) placed before any counterfactual or claim?
4. Does every gain have a number, named baseline, and regime?
5. Is the gain located where it is largest and where it vanishes?
6. Is one headline cross-checked independently?
7. Are anomalies and negatives reported?
8. Are headline numbers identical across sections?
