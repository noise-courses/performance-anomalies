# Grading rubric — Unsupervised Learning: PCA on Measuring Broadband America data

**10 points, graded for completion.** This is an optional/past assignment; it
is not graded unless the term page says otherwise. When it is assigned, the
same rule as the other assignments applies: if the notebook runs end to end
and each part does what it asks, you get full credit. The strength of the
relationships you find is *not* graded.

| # | Item | Pts |
|---|---|---|
| **Part 1 — PCA by hand** | | **3** |
| 1.1 | Center the toy dataset on its mean | 1 |
| 1.2 | Compute the covariance matrix of the centered data and its eigenvectors, sorted by eigenvalue | 1 |
| 1.3 | Project the data onto the eigenvectors and **plot** the result | 1 |
| **Part 2 — PCA on Measuring Broadband America data** | | **7** |
| 2.1 | Load and clean the throughput and latency measurements for the `sp2-vm-newyork-us.samknows.com` server into a dataframe | 1 |
| 2.2 | Merge on unit ID to get a mean throughput and mean latency per unit | 1 |
| 2.3 | Three relationship plots (latency vs. throughput, latency vs. DNS lookup time, latency vs. web page load time) **with a markdown answer** on what you observe and why | 1 |
| 2.4 | Per-unit averages of web page load time and DNS lookup time, merged with throughput and latency into a four-dimension matrix | 1 |
| 2.5 | **Describe the cleaning process** for the web and DNS data in a separate markdown cell | 1 |
| 2.6 | Pairwise 2-D plots of the four dimensions **with a written interpretation** of the relationships between speed, page load time, and DNS lookup time | 1 |
| 2.7 | Reduce the four-dimension matrix to two dimensions with PCA and **explain**, using the explained variance ratio, which features capture the most variance | 1 |

## Bonus (not part of the 10 points)

| # | Item | Pts |
|---|---|---|
| 3 | Part 3 (optional in the notebook): an unsupervised outlier-detection method over **at least two dimensions**, with a sentence on why the flagged points are real anomalies rather than one-dimensional extremes | bonus |

A good-faith attempt at Part 3 is noted in feedback; it does not change the
10-point score and skipping it costs nothing.

## Requirements that gate the score

- **The notebook must run.** Submit it *executed* (outputs saved). A notebook
  with error tracebacks in the cells that implement graded items, or with no
  outputs at all, is treated as not running: those items earn 0.5 until fixed
  and resubmitted.
- **Partial credit.** Each row is 1 point if done in good faith, 0.5 if
  attempted but incomplete or partly wrong, 0 only if absent. "Did the thing"
  is the bar, and ties go to you.
- **Written answers count.** Items 2.3, 2.5, 2.6, and 2.7 require a few
  sentences of explanation in a markdown cell, not just code and plots.
- **AI use.** Encouraged, but acknowledge it in the notebook and be ready to
  explain your code. Not acknowledging AI use does not cost points on this
  assignment, but see the syllabus on assessment of understanding.

## Late policy

Due 11:59 p.m. Chicago time on the due date; 96-hour grace balance for the term,
then half credit within one week, then zero. See the syllabus.
