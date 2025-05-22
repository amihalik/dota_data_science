# Data Overview

This report summarizes the datasets found in the `data/` directory and extracts key competition information from `README.md`.

## Dataset Files

| File | Size | Format |
|-----|-----|-------|
| sample_submission.csv | 264 bytes | CSV |
| test_features.csv | 0 bytes | CSV |
| training_features.csv | 0 bytes | CSV |
| training_targets.csv | 0 bytes | CSV |

## Dataset Summaries

### sample_submission.csv

Shape: 5 rows × 2 columns
| Column | Type | Nulls | Unique | Statistics |
|-------|------|-------|--------|------------|
| match_id_hash | object | 0 | 5 | - |
| radiant_win | object | 0 | 2 | - |

### test_features.csv

Shape: 0 rows × 0 columns
No columns (empty file).

### training_features.csv

Shape: 0 rows × 0 columns
No columns (empty file).

### training_targets.csv

Shape: 0 rows × 0 columns
No columns (empty file).

## Competition Details

**Objective**

Predict the binary target `radiant_win` for each match in the test set.

**Evaluation Metric**

Submissions are scored using the F1-score which balances precision and recall:

```
F1 = 2 * (precision * recall) / (precision + recall)
```

**Submission Format**

Create a CSV file with two columns:

```
match_id_hash,radiant_win
abcdef1234567890abcdef1234567890abcdef12,True
...
```
The file must contain a prediction for each match in the provided test set.
