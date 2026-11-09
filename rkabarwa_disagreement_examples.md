# Disagreement Examples: rkabarwa (validator) & emolder (author)

Projects come from emolder's MiniProject2. Between us there were 13 disagreements out of 50 records. All 13 are listed in
`rkabarwa_disagreement_resolution.csv`. The four below each show a different kind of disagreement.

## Example 1: secure-compilation/different_traces (HasRecovered, ActivityPattern)
**Parties:** emolder (author), rkabarwa (validator)
**Author:** HasRecovered = Partial; ActivityPattern = declining
**Validator:** HasRecovered = No; ActivityPattern = stopped
**Evidence:** The project had 219 commits in 2018 and 289 in 2019, both tied to the ESOP 2020 paper. It had 10 in 2020,
the last on 2020-08-04, followed by a 1,738-day gap. The only later commit (2025-05-08) adds contributor credits to the README.
**Discussion:** "Partial" is not a codebook value. On the other log we had already agreed that a single README or packaging
commit after a gap (riatelab_cartography, patrickzib_sfa) is not recovery, and the same rule applies here. Without a
recovery, "stopped" describes the curve better than "declining".
**Resolution:** ValidatorKept (No / stopped). Currentstatus stays Active only because of the 6-month date rule.

## Example 2: cgre-aachen/gempy (ActivityPattern)
**Parties:** emolder (author), rkabarwa (validator)
**Author:** declining
**Validator:** U-shaped
**Evidence:** Yearly commits were 1003 (2020), 134 (2021), 62 (2022), 536 (2023), 245 (2024), and 360 (2025).
**Discussion:** The author read the drop after the 2020 peak as a decline. Activity in 2023-2025 is well above the 2021-2022
low, so the curve dips and then recovers.
**Resolution:** ValidatorKept (U-shaped).

## Example 3: pekkosk/hotbit (WhyRecovered)
**Parties:** emolder (author), rkabarwa (validator)
**Author:** Later commits fixed orbital/energy bugs.
**Validator:** Owner set up GitHub Pages docs (Dec 2015).
**Evidence:** The first commits after the 846-day gap (2015-12-10) are by pekkosk: removing the build directory, adding
parameters, and creating GitHub Pages and README material. The orbital/energy fixes (Markus Kari) came years later.
**Discussion:** Both answers were true but described different moments. The trigger is the first return, and the bug fixes
are part of the longer recovery, so we listed both in date order.
**Resolution:** Compromise. "Original maintainer returned in Dec 2015 (build cleanup, parameters, GitHub Pages docs); new
contributors later fixed orbital/energy bugs."

## Example 4: digantamisra98/Mish (HasRecovered, WhyRecovered)
**Parties:** emolder (author), rkabarwa (validator)
**Author:** HasRecovered = Yes; WhyRecovered = maintainer resumed README/citation updates
**Validator:** N/A for both
**Evidence:** The longest gap before the 2025-09-30 cutoff is 41 days, and emolder's own stats file lists 0 gaps. The
Dec 2025-Jan 2026 pause falls after the cutoff.
**Discussion:** A project cannot recover without a qualifying gap, so WhyRecovered follows HasRecovered.
**Resolution:** ValidatorKept (N/A, N/A).
