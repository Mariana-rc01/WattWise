# Analysis of Self-Consumption Energy Systems in Portugal (2023–2024)

## Overview

This project investigates the deployment and growth of **Total Production Units for Self-Consumption (UPACs)** in Portugal during 2023–2024. Using a comprehensive dataset from **e-Redes**, the study examines how **regional, seasonal, and technical factors** shape the distribution and evolution of residential and industrial self-consumption energy systems.

The analysis combines **descriptive statistics**, **exploratory data analysis**, and **inferential techniques** (e.g., t-tests, ANOVA, Levene’s test) to provide a rigorous, evidence-based view of Portugal’s decentralized energy landscape. The findings reveal a dual structure of small residential systems and large industrial units, strong regional disparities, and minimal seasonal variation.

---

## Project Structure

The project follows a **six-step statistical research methodology**, adapted to a data-driven perspective:

1. **Data Collection & Study Design**

   * Dataset: [e-Redes – Total Production Units for Self-Consumption](https://e-redes.opendatasoft.com/explore/dataset/8-unidades-de-producao-para-autoconsumo/information/)
   * Years: 2023–2024
   * Key variables: installed capacity (kW), voltage level, district, municipality, quarter, year

2. **Research Questions**

   * **General RQ:** How do seasonal, regional, and power-level factors shape self-consumption patterns in Portugal (2023–2024)?
   * **RQ1:** Compare total installed capacity across districts between 2023 and 2024.
   * **RQ2:** Compare evolution of installed capacity across residential vs. industrial UPACs.
   * **RQ3:** Assess seasonal and power-scale patterns in total installed capacity across selected districts.

3. **Data Exploration and Cleaning**

   * Translation of column names
   * Removal of duplicates and missing values
   * Log-transformations and robust statistical adjustments for skewed distributions

4. **Descriptive and Inferential Analysis**

   * Summary statistics and visualizations of installed capacities
   * ANOVA, Welch’s t-tests, Levene’s test for variance homogeneity
   * Post-hoc pairwise comparisons to detect significant differences

5. **Conclusions**

   * **Temporal trends:** Strong year-on-year growth in UPAC capacity
   * **Sectoral patterns:** Industrial UPACs dominate capacity; residential systems are numerous but smaller
   * **Regional effects:** Capacity distribution varies across districts, reflecting socio-economic and infrastructural factors
   * **Seasonal impact:** Minimal effect on installed capacity

6. **Reflection and Future Directions**

   * **Challenges:** Managing a large dataset, skewed distributions, multidimensional analyses
   * **Future work:**

     * Extend temporal coverage and forecast growth
     * Integrate socio-economic and demographic indicators
     * Link capacity data with generation performance and environmental impact

---

## Key Insights

* Portugal’s self-consumption sector exhibits a **bifurcated structure**: small, widespread residential units vs. large, concentrated industrial systems.
* Regional disparities remain significant, indicating uneven adoption across districts.
* Growth between 2023 and 2024 is **structural**, not seasonal, highlighting long-term investment trends.
* Voltage level and system scale are **key determinants** of installed capacity distribution.

---

## Requirements

* Python 3.10+
* Common data science libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`

---

## How to Use

1. Clone this repository.
2. Load the **e-Redes UPAC dataset** into the `data/` folder.
3. Run `data_cleaning.ipynb` to prepare the dataset.
4. Explore descriptive statistics and visualizations in `exploratory_analysis.ipynb`.
5. Run `inferential_analysis.ipynb` for hypothesis testing and model results.
6. Review `conclusions_and_visuals.ipynb` for integrated insights and figures.

---

## References

* e-Redes Open Data Platform: [Total Production Units for Self-Consumption](https://e-redes.opendatasoft.com/explore/dataset/8-unidades-de-producao-para-autoconsumo/information/)
* Portugal’s National Energy and Climate Plans
* Statistical methods: t-test, ANOVA, Levene’s test, post-hoc pairwise comparisons
