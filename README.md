# **Project Title: Larvicide Efficacy Analysis Pipeline**

## **Overview**

This repository demonstrates an end-to-end statistical analysis and reporting pipeline developed for a client. Using **R** and **Quarto**, the system processes raw experimental data from pesticide trials to assess the efficacy of larvicide treatments on *Anopheles* populations.

## **The Science**

The study evaluates mortality rates of *Anopheles quadrimaculatus* (third instar larvae) over a 96-hour period. The goal is to determine treatment effectiveness through statistical comparison against control groups while identifying and handling experimental outliers.

## **Data Simulation**

To maintain client confidentiality, this portfolio project utilizes an anonymized, **synthetic dataset**. The actual test sample name was replaced with "TREATMENT".

-   **Data synthesis:** Included in this repo is `create_synthetic_data.qmd`, which uses the package `synthpop` to generate a synthetic dataset with the same distribution of mortality values (per treatment) as the original data.

-   **Validation:** The `synthpop` package includes functions to compare the original and synthetic data through visualizations and pMSE, the propensity mean squared error, a measure of the utility of synthetic data based on how distinguishable it is from the original, real data. Plots were inspected but not included here to maintain confidentiality.

## **Key Features**

-   **Reproducible Research:** The Quarto workflow ensures that results and and statistical tables are generated directly from the data.

-   **Automated Data Validation:** Built-in logic to flag replicates that fail quality control (QC) metrics.
