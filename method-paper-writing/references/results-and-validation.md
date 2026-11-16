# Results and Validation Guide (Method Papers)

## Principle

Results follow the track and question. Explain why key results arise. Present relevant model checks before body counterfactuals that rely on them; truthful abstract and introduction previews can appear earlier.

## Theory Arc

**Source and variation.** The benchmark, main proposition, comparative statics, and extensions follow the theory exemplar; a later analytical exemplar also pairs proposition and interpretation. The order and count of numbered results are adaptable, and the benchmark need only precede the result it clarifies.

1. **Benchmark model result:** what happens without the key force. This is the default the main result deviates from.
2. **Main result,** with a precise formal statement and nearby economic explanation. Keep a proof or derivation in the body when it clarifies the central construction; otherwise give a verified proof pointer. Interpretation may precede the result or follow a short proof. See [Theorem Statements and Proofs](theorem-and-proof-style.md) for characterization and equivalence routes and appendix proof craft.
3. **Comparative statics with economic explanation:** state formal directions and explain the driving forces nearby; flag counterintuitive ones when present.
4. **Dichotomy check, when the model explains two observed regimes:** both arise in different parameter regions. Otherwise, check that the formal result answers the stated question under its assumptions.
5. **Extensions** with propositions where the claim needs them. Irrelevance results are results.
6. **Research questions** from the introduction are answered by formal results or explanatory prose as appropriate.

For a theory paper whose headline is a capability or sufficiency result, see the adapted capability-results route below.

The statement and proof patterns for characterization and equivalence results have direct theory-corpus support. The broader capability-results route below remains an editorial adaptation; this evidence does not establish its learning-time, computation-limit, or rate-related sequence.

### Adapted Capability-Results Route

**Editorial adaptation (unverified extrapolation).** The source corpus shows enabling-method rhetoric, but no capability-theorem results template. For a headline capability or sufficiency result, a useful route is: question → precise guarantee and conditions → mechanism → existing bound components and their units → learning-time and computation limits, including what is not established (such as a rate) → supported consequence. Explain only bounds and limits the paper establishes; this route does not require a new rate, a percentage gain, or a numerical cross-check the paper does not have.

## Structural Arc

**Source and variation.** Estimates, fitted-sample model checks, within-regime simulations, and regime changes follow the structural exemplar. Conditional counterfactual interpretation recurs in the hybrid analytical paper. Independent policy evaluation is a separate empirical design, not an implied feature of this arc.

1. **First-stage estimates** briefly; details to the appendix.
2. **Structural parameters against restricted models** when a bias or fit comparison is claimed; use a table when it clarifies the contrast.
3. **An economic story for material parameters,** tied to the vocabulary of the introduction.
4. **Fit and model checks** using the evidence actually available. Fitted-sample predicted-versus-observed comparisons are not independent held-out or untargeted evaluation. Add independent checks when the claim requires them, before body counterfactuals that rely on the model.
5. **Within-regime simulations** that monetize the estimates.
6. **Regime-change counterfactuals** framed as plain-language manager questions. Each pairs a (possibly surprising) result with its mechanism and a recommendation. State partial-equilibrium caveats, and recast estimates as bounds where honest.

## ML-Method Arc

**Source and variation.** Tested pure-method diagnosis, hybrid comparisons by horizon, ablation, and costs follow the ML-method exemplar. Claim-specific benchmarks recur across method papers. The figure/table arrangement and exact position of cost reporting are editorial options.

1. **Top-line claim:** summarize supported performance across the tested regimes, using figures and pairwise comparisons where informative.
2. **Versus each pure approach,** with the mechanism of the gain explained and its trajectory across regimes (horizon, traffic, sample size).
3. **Where the gain is largest,** aligned with the regime the manager cares about.
4. **Embedded managerial finding, when supported:** describe the comparison with the status-quo practice.
5. **Ablations** testing the design intuition; report improvements or reversals from removal as well as losses.
6. **Cost and runtime accounting** when the advantage or implementation claim depends on them.
7. **Honest negatives:** regimes without a significant gain are reported as such.

## Shared Rules

1. For a quantitative gain claim, give a number, named baseline, and relevant regime together. A formal capability claim needs a precise theorem and conditions instead of an invented percentage.
2. Repeat headline numbers consistently where the paper makes quantitative claims.
3. Cross-check a headline result independently when claiming corroboration or when model dependence makes that check material.
4. Surface and resolve anomalies; never bury them.

## Checklist

1. Does the results section follow the arc of the paper's track?
2. Are key results explained economically, with paragraph length suited to their complexity?
3. Are fitted-sample checks, independent evaluations, benchmarks, and limiting cases labeled correctly? Do relevant checks precede body counterfactuals built on them, while introductory previews remain truthful?
4. Do quantitative gain claims have a number, named baseline, and regime? If not applicable, record `not applicable — reason`.
5. For comparative performance claims, is the gain located where it is largest and where it vanishes when relevant?
6. Is an independent cross-check present when the paper claims one or relies on it for credibility?
7. Are anomalies and negatives reported?
8. Are headline numbers substantively consistent across sections, allowing compatible rounding?
