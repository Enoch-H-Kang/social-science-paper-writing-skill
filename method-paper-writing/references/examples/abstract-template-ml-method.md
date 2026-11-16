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

1. `Firms that [task] must balance [cost A] against [cost B].`
2. `Using [large archive from SETTING], we evaluate [three pure approaches] on [task].`
3. `[Approach 1] performs near chance, [approach 2] does better, and [approach 3] does best, yet [none reaches the level a manager needs].`
4. `Thus, [approach family] cannot replace [current practice] on its own.`
5. `We propose [FRAMEWORK NAME], which [combines X with Y].`
6. `[FRAMEWORK] uses [predictions] as [priors/inputs] so that [failure mode of incumbent] is removed.`
7. `It outperforms [pure approach], [classical algorithm], and [firm's status-quo practice] by [X%], [Y%], and [Z%], especially when [scarce resource].`
8. `The approach extends to [adjacent settings], and [cost / privacy / compatibility note].`

## Usage rules

1. The negative result is ranked, not asserted: say which approach loses and by how much.
2. Every percentage names its baseline; include the status-quo practice among the baselines.
3. The framework's name appears once.
4. Reuse the sentence logic, not the wording.

## Checklist

1. Is the failure of the pure approaches stated with a ranking?
2. Is the regime boundary ("especially when…") present?
3. Is the status-quo practice among the named baselines?
