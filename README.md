# ICU Infection Prevention Adherence: Extended Python Analysis

Code and extended statistical analysis for our multi-center study on device-associated infection prevention measures in Intensive Care Units. 

## Status Update (March 2026)
Our main article, ***Assessment of Awareness, Adherence, and Barriers to Device-Associated Infection Prevention Measures in Intensive Care Units: A Multi-Center Cross-Sectional Study***, has been accepted and published online (in press) by the *American Journal of Infection Control*.
* [Article Link (AJIC)](https://www.ajicjournal.org/article/S0196-6553(26)00100-8/abstract)
* [ScienceDirect Link](https://www.sciencedirect.com/science/article/pii/S0196655326001008?dgcid=author)

---

## Project Context & Motivation

The original statistical analysis for the manuscript was conducted using SPSS. As the corresponding author, I created this repository with two main goals:
1. **Transparency & Reproducibility**
2. **Extended Analysis**: To explore the data beyond the scope of the published paper. The notebooks here include additional inter-rater reliability checks (Attending vs. Head Nurse) and more granular data visualizations that didn't make it into the final manuscript due to space constraints.

## Repository Structure

The analysis is broken down into four Jupyter notebooks to keep the workflow readable:

- `descriptive_statistics.ipynb`: Data loading, cleaning, and basic distributions across the 20 participating ICUs (General, Surgical, Medical). Looks at the highest and lowest adherence items among the 116 questionnaire variables.
- `inferential_statistics.ipynb`: Explores correlations between adherence to different prevention bundles (CLABSI, CAUTI, VAP). Includes ANOVA testing across ICU types (note: includes Levene's test for variance homogeneity, utilizing Welch's ANOVA where assumptions failed).
- `inferential_statistics2.ipynb`: A deeper dive into inter-rater consistency using paired samples t-tests and Pearson correlations to see if Attending Physicians and Head Nurses perceived adherence differently.
- `data_visualizations.ipynb`: Contains the code for generating the distribution boxplots/stripplots and ICU ranking visualizations. 

## The Data

The `data/` directory contains the aggregated datasets used for this analysis. To protect participant anonymity, only aggregated mean scores at the ICU level (and rater level) are included.
* `icu_adherence_by_rater.csv`: Mean bundle scores categorized by ICU and rater.
* `icu_adherence_by_item.csv`: Item-level adherence scores across the ICUs.

## Requirements
To run these notebooks locally, you'll need standard data science libraries:
`pip install pandas numpy matplotlib seaborn scipy statsmodels`