# New Features Overview

**Goal:** Summarize and consolidate docket-level variability into meaningful, case-level metrics for analysis.

## 1. Number of Dockets (`num_dockets`)
- **Definition:** Total count of dockets associated with each case.
- **Purpose:** Provides an indication of the case’s complexity or scope, as more dockets often involve more issues or deliberation.

---

## 2. Entropy for Each Column (`[column]_entropy`)
- **Definition:** Measures the variability or diversity of categorical values across dockets for a specific column (e.g., `lawType`, `issue`).
- **Interpretation:**
  - **Low Entropy:** Values are consistent across dockets (e.g., all dockets share the same `lawType`).
  - **High Entropy:** Values vary significantly across dockets, indicating diversity in the feature.

---

## 3. Most Frequent Value (`[column]_most_frequent`)
- **Definition:** Identifies the value that appears most frequently across dockets for a given column.
- **Purpose:** Provides a "representative" value that summarizes the dominant characteristic of the case for that feature.

---

## 4. Revised Dominance Score (`[column]_dominance_score`)
- **Definition:** Quantifies how strongly the most frequent value dominates other values within a case, adjusted for the total number of dockets.
- **Calculation:**
  - Scales the dominance score (proportion of the most frequent value) by the number of dockets.
  - Reduces the score to `0` if the most frequent value isn’t strongly dominant (e.g., an even split).
- **Interpretation:**
  - **Higher Scores:** Indicates a single value dominates the case.
  - **Score of 0:** Reflects no clear dominance (e.g., values are evenly distributed).

---

## Why These Features Matter
- **Simplifies Analysis:** Consolidates docket-level data into case-level summaries, reducing complexity.
- **Preserves Key Information:** Retains variability, trends, and patterns across dockets.
- **Enhances Interpretability:**
  - **Entropy:** Captures variability in issues or legal provisions.
  - **Most Frequent Value:** Highlights dominant trends within a case.
  - **Revised Dominance Score:** Differentiates between ambiguous and clear-cut cases.
