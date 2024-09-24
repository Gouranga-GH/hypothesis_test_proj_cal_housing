
# California Housing Dataset Analysis

This repository contains an analysis of the California Housing dataset. The objective is to explore and validate various hypotheses regarding factors that influence housing prices in California.

## Problem Statement

The main goal is to predict the median house value in various districts of California based on several features such as the median income, housing median age, total rooms, total bedrooms, population, households, latitude, and longitude. By building a predictive model, we aim to understand the relationship between these features and the house prices, which can help in making informed decisions in real estate investments, urban planning, and policy-making.

The goal of the analysis here is to **understand key factors influencing house values in California** and **validate assumptions** about relationships between different features and the target variable, `Median House Value`. Additionally, the analysis investigates whether population or geographic features significantly affect housing prices.

## Framework Overview

1. **Understand the Problem**: Brief overview and identification of key factors.
2. **Generate Hypotheses**: Establish assumptions about the data.
3. **Test Hypotheses**: Apply statistical tests to validate or reject hypotheses.
4. **Summarize Results**: Draw conclusions based on the tests.

## Dataset

The dataset used in this project is the California Housing dataset from the `sklearn` library. It includes features such as:
- Median income (`MedInc`)
- Median house age (`HouseAge`)
- Average rooms per household (`AveRooms`)
- Average bedrooms per household (`AveBedrms`)
- Population
- Latitude
- Longitude
- Target variable: `Median House Value`

## Hypotheses

We have formulated **11 hypotheses** related to different features in the dataset. These hypotheses are tested using various statistical methods.

### Hypothesis List

1. **H1**: Median house values are higher in areas with higher average income.
2. **H2**: Proximity to the ocean (measured by latitude) affects house prices.
3. **H3**: House age is related to population size.
4. **H4**: Inland areas (low latitude) have lower housing prices compared to coastal regions.
5. **H5**: Areas with higher total rooms have higher median house values.
6. **H6**: The number of bedrooms per house differs across geographical areas.
7. **H7**: Older houses (median house age) have lower prices than newer houses.
8. **H8**: High-income areas have a significantly lower population density.
9. **H9**: The total number of rooms per household is similar to the total number of bedrooms per household.
10. **H10**: There is no significant difference in housing prices between areas with high and low population densities.
11. **H11**: The distribution of house values is not normal (test for normality).

## List of Statistical Tests Used

1. **Pearson Correlation Test**: Used to test the linear relationship between two continuous variables (e.g., `MedInc` and `Median House Value`, `HouseAge` and `Population`).
2. **ANOVA (Analysis of Variance)**: Used to test for significant differences between groups (e.g., `Latitude` and `Median House Value`).
3. **T-Test (Independent)**: Used to compare means between two independent groups (e.g., house prices between inland and coastal regions).
4. **Paired T-Test**: Used to compare means between two related groups (e.g., total rooms and total bedrooms per household).
5. **Chi-Square Test**: Used to test associations between categorical variables (e.g., bedrooms distribution across different geographic regions).
6. **Z-Test**: Used to compare population means when the population variance is known (e.g., population density between high and low-income areas).
7. **Shapiro-Wilk Test**: Used to test the normality of the distribution of a variable (e.g., normality of `Median House Value`).


## Installation & Setup

1. Clone the repository:

   \`\`\`bash
   git clone https://github.com/your-username/california_housing_analysis.git
   cd california_housing_analysis
   \`\`\`

2. Install the required dependencies:

   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`

3. Open the notebook in Jupyter or Google Colab to explore the analysis:

   \`\`\`bash
   jupyter notebook california_housing_analysis.ipynb
   \`\`\`

## Dependencies

The analysis uses the following Python libraries:

- \`pandas\`
- \`numpy\`
- \`matplotlib\`
- \`seaborn\`
- \`scipy\`
- \`sklearn\`
- \`statsmodels\`

Make sure to install these libraries using the \`requirements.txt\` file.

## Summary of Hypothesis Tests

1. **H1**: A strong positive correlation between income and house values.
2. **H2**: Latitude significantly affects house prices, with coastal regions showing higher prices.
3. **H3**: Negative correlation between house age and population size.
4. **H4**: Coastal areas have significantly higher house prices than inland areas.
5. **H5**: Total rooms are positively correlated with house values.
6. **H6**: No significant difference in bedroom distribution across regions.
7. **H7**: Older houses tend to have lower prices than newer houses.
8. **H8**: High-income areas have lower population density.
9. **H9**: Significant difference between the number of rooms and bedrooms per household.
10. **H10**: No significant difference in house prices between high and low population density areas.
11. **H11**: The distribution of house values is not normal.

## Conclusion

The analysis provides insights into the factors that influence housing prices in California, confirming that income, proximity to the ocean, and the number of rooms significantly impact house values. This analysis also highlights geographic and population-related trends.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
