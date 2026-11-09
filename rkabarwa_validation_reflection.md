# Validation Reflection: rkabarwa

I validated ten projects from emolder's MiniProject2. Before discussion we agreed on 37 of 50 records (74%). The
mechanical field, Currentstatus, matched on all ten projects. Agreement was lowest for the interpretive fields:
ActivityPattern (60%, κ = 0.245) and WhyRecovered (60%). HasRecovered reached 70%, but κ was only 0.388, because most
projects were "Yes" and chance agreement was therefore high. After discussion all 13 disagreements were resolved. Eleven kept
the validator's value, two were compromises written for WhyRecovered (minmea, hotbit), and none kept the author's original value unchanged.
Our decisions were consistent with the AuthorKept outcomes in emolder's log, where I was the author. The same rules decided
both logs.

The adjudicated labels show some patterns in what comes before long gaps. In several projects the last pre-gap commits mark
the end of a piece of work rather than a breakdown. different_traces stopped right after its ESOP 2020 camera-ready proofs.
denbi-nanopore-training stopped after its 2020 COVID course merge. gempy and e3nn paused after packaging, CI, and README
cleanup. A pre-gap stretch of nothing but documentation and release housekeeping was the most common warning sign. Activity
volume was a weaker signal: projects with 400 to 1000 commits a year still went quiet.

Recovery triggers were concrete events, not just time passing:
- A maintainer clearing a review backlog (minmea merged PR #58, which had been open since Nov 2020).
- A new contributor bringing a feature (e3nn's torch.compile support in PR #436; dnnbrain's CLIP and RSA modules).
- New course material (Bakta and EDGAR pages in denbi-nanopore-training).
- A maintainer returning to rebuild documentation and infrastructure (hotbit's GitHub Pages in Dec 2015).

When the person behind the recovery differed from the person before the gap, the recovery tended to last longer
(e3nn, dnnbrain, hotbit).

Gaps did not reliably mean a project had died. gempy dropped from 1003 commits in 2020 to 62 in 2022 and then returned to
several hundred a year, which is why it was relabeled U-shaped instead of declining. The reverse also held: the date rule
calls different_traces "Active" because of one README commit in 2025, yet its activity pattern is "stopped" and it did not
recover. Currentstatus and HasRecovered answer different questions, and a reader should not use the first to stand in for
the second.

Interpretation pitfalls came up repeatedly:
1. **Defaulting to "declining" for any curve that peaks early.** The author used it for 9 of 10 projects. Checking yearly
   counts against the codebook definitions separated declining from irregular, U-shaped, and stopped.
2. **Values outside the codebook.** "Partial" is not allowed for HasRecovered. We mapped it to Yes or No depending on
   whether the post-gap work was substantive, and recorded the qualification (for example, the branch-only recovery in
   denbi-nanopore-training) in Comments.
3. **Counting a single small commit as recovery.** We applied one rule to both logs: a lone README or packaging commit is
   not recovery.
4. **Mixing up the first post-gap event with later work** in WhyRecovered. We fixed this by putting events in date order.
5. **Choosing the wrong commit window for RecentThemes.** The codebook asks for the last 10 commits, not the commits after
   the gap. Merge commits needed to be read through to the underlying change.

A clearer codebook entry for "stopped" and an explicit rule for branch-only activity would have prevented about half of our
disagreements.
