# Repeated Design and Span Consistency

| Test ID | Objective | Compared input | Observed result | Status | Evidence |
| --- | --- | --- | --- | --- | --- |
| DES-04 | Check outputs after a span change | 31 m vs 32 m | Width 13.45→13.65 m; spacing 3.36→3.41 m; overhang 1.68→1.71 m; DL 38.592→39.17 | PASS | Generic archive has comparison tables; exact one-to-one mapping not confirmed |

Changing span provides a controlled way to see whether later geometry and load outputs follow the updated configuration. The observed values changed consistently in the recorded comparison. The evidence does not establish a complete three-run sequence, all-output consistency, or independent correctness of each dimension and load.

**Reproducibility note:** the QA workbook explicitly says a complete three-run baseline/geometry/material sequence was not evidenced. The 31 m/32 m comparison is documented as its own test and should not be described as a full three-run persistence test.
