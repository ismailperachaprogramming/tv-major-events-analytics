# TV Major Narrative Events – Rating Impact Analysis

## Overview
This project analyzes whether major narrative events in television episodes, such as character deaths, cast exits, premieres, and finales, correlate with higher audience ratings.  

Using a structured episode-level dataset, this analysis applies statistical testing and visualization techniques to determine whether pivotal storytelling moments influence viewer reception.

---

## Dataset Source

This project uses the **TV Episode Major Events Dataset**, which contains episode-level metadata and event classifications across multiple television series.

**Dataset Repository:**  
https://github.com/ismailperachaprogramming/tv-major-events-dataset

The dataset includes:
- Episode ratings
- Air dates
- Event classifications
- Controlled vocabularies
- Priority logic for event selection

---

## Research Question
**Do episodes marked as major narrative events receive higher IMDb ratings than non-event episodes?**

---

## Methodology

### 1. Data Preparation
- Loaded `episodes.csv`
- Converted rating fields to numeric
- Split data into two groups:
  - Event episodes (`is_event = 1`)
  - Non-event episodes (`is_event = 0`)

### 2. Statistical Testing
- Calculated mean and median ratings
- Performed a **two-sample t-test** to evaluate statistical significance

### 3. Visualization
- Box plot comparing rating distributions
- Bar chart of mean ratings

---

## Key Findings

- **Average rating (Event Episodes): 8.7**
- **Average rating (Non-Event Episodes): 8.4**
- **p-value:** 0.00017

The extremely low p-value indicates the difference is statistically significant, suggesting that major narrative events are associated with higher audience ratings.

---

## Tools Used
- Python
- pandas
- matplotlib
- scipy
- Jupyter Notebook

---

## Conclusion
The analysis indicates a meaningful relationship between pivotal narrative moments and audience reception. This project demonstrates how structured event tagging combined with statistical analysis can uncover patterns in media storytelling and viewer behavior.
