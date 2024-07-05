# Used Car Pricing Optimization

## Overview

This project aims to optimize used car pricing strategies for dealerships using advanced regression modeling techniques. By analyzing a dataset with extensive vehicle attributes, including year, mileage, drive type, engine size, fuel type, and transmission, we seek to provide insights that help dealerships maximize profitability and inventory turnover.

## Summary of Findings

After extensive data collection, organization, and analysis, the key findings are as follows:

- **Optimal Attributes**: Dealerships should prioritize the following attributes to maximize vehicle sale prices:
  1. Year of the vehicle (newer vehicles fetch higher prices).
  2. Odometer reading (lower mileage correlates with higher prices).
  3. Drive type (forward or rear-wheel drive often commands higher values).
  4. Cylinder count (larger engines typically result in higher prices).
  5. Fuel type (gasoline-powered vehicles generally have higher resale values).
  6. Transmission type (automatic transmissions positively impact vehicle prices).

- **Model Selection**: A polynomial regression model of degree 3 was selected as the optimal predictive model, balancing accuracy with computational feasibility.

- **Limitations and Future Directions**: The model does not account for expected profit margins and inventory turnover impacts. Future enhancements could include incorporating profitability metrics and exploring alternative modeling techniques like logarithmic transformations for improved inference accuracy.

## Recommendations

Based on the findings, the following recommendations are proposed for dealership optimization:

1. Implement the polynomial degree 3 regression model for pricing predictions.
2. Collect additional data on profitability metrics and inventory turnover for comprehensive optimization strategies.
3. Consider alternative modeling approaches to refine price prediction accuracy, such as logarithmic transformations.
4. Communicate insights in non-technical language to dealership stakeholders for informed decision-making.

## Project Organization

- **README**: This file contains a summary of findings and recommendations for dealership optimization. [Link to README.md](./README.md)

- **Jupyter Notebook**: The notebook `https://github.com/AparnaPillai46/What_Drives_Price_Of_A_Car/blob/main/practical_application_II_starter/prompt_II.ipynb` includes headings and formatted text to facilitate easy reading and understanding of the analysis.

- **Files**: No unnecessary files are included in the project directory. All directories and files are appropriately named and located for clarity and organization.

## Usage

To replicate the analysis:

1. **Data**: Obtain a dataset containing detailed vehicle attributes.
2. **Preprocessing**: Clean and prepare the data, handle missing values and categorical variables appropriately.
3. **Modeling**: Implement polynomial regression models of varying degrees and evaluate their performance using metrics like MSE, MAE, and R² score.
4. **Analysis**: Interpret the model results, identify impactful features, and derive actionable insights for dealership strategies.
