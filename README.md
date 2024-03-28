# Assessment 1 - Ensamble Learning - Machine Learning II

# Estimating Hourly Utilization from Available Variables

## Objective
The objective of this project is to estimate the hourly utilizations of a day based on the available variables. This involves utilizing ensemble techniques and comparing them with more direct methods. Additionally, a fair validation will be conducted to select the best approach among those attempted.

## Contents
1. **Introduction**: A brief overview of the project's objectives and methodologies.
2. **Exploratory Data Analysis (EDA)**: Preliminary analysis to understand the data and its distributions, correlations, and anomalies.
3. **Methodology**: Description of the ensemble techniques and direct methods used for estimating hourly utilizations.
4. **Validation**: Details about the validation process employed to select the best-performing approach.
5. **Results**: Presentation of results, including comparisons between different methods and insights gained.
6. **Examples of Poorly Estimated Cases**: Illustrative examples showcasing instances where estimations were inaccurate and potential reasons behind them.
7. **Conclusion**: Summary of findings and conclusions drawn from the analysis.

## Delivery
- **Report**: The report will be provided in PDF format, covering all aspects of the project.
- **Jupyter Notebooks**: Notebook/s used for the analysis will be provided, organized similarly to the structure of the report.

---

**Introduction**

Solar energy, with its immense potential for sustainability and renewable power generation, has garnered increasing attention as a viable alternative to traditional energy sources. In the pursuit of harnessing solar energy effectively, understanding and predicting solar irradiation—the amount of solar energy received per unit area—play crucial roles. Solar irradiation serves as a primary determinant of solar energy utilization, influencing various applications such as power generation, agriculture, and environmental management.

In this project, we focus on forecasting solar energy utilization in a specific region by leveraging ensemble learning methods. Our dataset spans the years 2015 to 2020 and comprises several variables, including timestamps, solar irradiation measurements at three-hour intervals throughout the day, and additional temporal features. The core objective is to predict solar energy utilization, which is intricately linked to solar irradiation and temporal factors.

**Dataset Description**

The dataset consists of the following columns:

- **FECHA**: Timestamps representing the date and time of each observation.
- **IRRADH00** to **IRRADH21**: Solar irradiation measurements at three-hour intervals throughout the day.
- **ANNO**: Year component extracted from the timestamps.
- **MES**: Month component extracted from the timestamps.
- **DIA**: Day component extracted from the timestamps.
- **DIASEM**: Day of the week extracted from the timestamps.

These columns collectively provide comprehensive temporal coverage and solar irradiation data, essential for modeling and forecasting solar energy utilization.

**Objective**

Our primary objective is to develop predictive models for solar energy utilization based on solar irradiation and temporal features. Specifically, we aim to establish a functional relationship between solar irradiation (Irr) and solar energy utilization (Ud,h), where Ud,h represents the utilization at a given timestamp. This relationship is expressed as Ud,h = f(Irr, fecha), indicating that solar energy utilization is a function of solar irradiation and time.

**Approach**

To achieve our objective, we will employ ensemble learning methods, which combine multiple base models to enhance predictive performance and robustness. Ensemble methods, such as Random Forests, Gradient Boosting, and Stacking, are well-suited for handling complex relationships and capturing nonlinearities present in solar energy utilization patterns.

By leveraging the temporal dynamics encoded in the dataset and the predictive power of ensemble learning, we aim to build accurate and reliable models for forecasting solar energy utilization. These models have the potential to inform decision-making processes, optimize energy management strategies, and contribute to the sustainable utilization of solar resources.