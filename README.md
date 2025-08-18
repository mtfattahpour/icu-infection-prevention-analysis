# Analysis of Adherence of ICUs to Infection Prevention Measures

This repository is for a statistical analysis of data from a cross-sectional and multi-center study on adherence to device-associated infection prevention measures in intensive care units that we conducted recently.

## Repository Purpose

The original statistical analysis for this research paper was conducted using SPSS, but my goal with this repository is to use a programmatic approach to redo the same analyses in Python, to extend the analyses and exploration of data far beyond the scope of the analyses included in the paper, and also offer greater transparency, reproducibility as well as more sophisticated visualization methods to capture more nuances.

## Datasets

The `data` directory contains the two primary datasets from our research.

* `icu_adherence_by_rater.csv`: Contains the mean adherence scores for the three main infection prevention categories, Central Line-Associated Bloodstream Infection (CLABSI), Catheter-Associated Urinary Tract Infection (CAUTI), Ventilator-Associated Pneumonia (VAP), as assessed by two raters (Head Nurse and Attending Physician) across the 20 participating ICUs.
* `icu_adherence_by_item.csv`: Contains the granular, item-level adherence scores for each of the 116 specific practices assessed, averaged per ICU.
* `questionnaire_items.md`: A reference file listing the 116 questionnaire items.
* `icu_list.md`: A reference file listing the 20 participating ICUs.
