# Abstract Template: ML Method (Diagnose and Hybridize)

Eight slots. Content is generic and invented; replace every bracket.

```latex
\section{Abstract}
% Managerial need
% Data + evaluation of the pure approaches
% Ranked negative result
% Verdict sentence (the empirical contribution in one line)
% Method announcement (named framework)
% Mechanism in one line
% Win vs. named baselines, incl. the status quo; regime boundary
% Scope / generalizability close
```

## Reusable skeleton

1. `Firms need [efficient way to complete task] in [setting].`
2. `Using [large archive from SETTING], we evaluate [three pure approaches] on [task].`
3. `[Approach 1] performs near chance, [approach 2] does better, and [approach 3] does best, yet [none reaches the level a manager needs].`
4. `Thus, [approach family] cannot replace [current practice] on its own.`
5. `We propose [FRAMEWORK NAME], which [combines X with Y].`
6. `[FRAMEWORK] uses [predictions] as [priors/inputs] to [reduce or correct the specified obstacle to the supported degree].`
7. `It outperforms [named pure approach], [named algorithm], and [status-quo practice if tested], especially when [identified resource is scarce].` Add percentages only when the abstract reports them, with a named baseline for each.
8. `The approach extends to [adjacent settings], and [cost / privacy / compatibility note].`

## Usage rules

1. State the negative result for the tested methods and task; rank approaches and quantify the gap when the evidence supports it.
2. Every percentage names its baseline; include the status-quo practice when it was evaluated.
3. The framework's name appears once.
4. Reuse the sentence logic, not the wording.

## Checklist

1. Is the obstacle established for the methods and task actually tested?
2. Is the regime boundary ("especially when…") present?
3. Are the named baselines and performance claims the ones the paper evaluates?
