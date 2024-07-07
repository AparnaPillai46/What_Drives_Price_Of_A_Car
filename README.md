# Used Car Pricing Optimization

## Overview

This project aims to optimize used car pricing strategies for dealerships using advanced regression modeling techniques. By analyzing a dataset with extensive vehicle attributes, including year, mileage, drive type, engine size, fuel type, and transmission, we seek to provide insights that help dealerships maximize profitability and inventory turnover.

## Project Organization

- **Jupyter Notebook**: The [Link to notebook](./practical_application_II/prompt_II.ipynb) includes headings and formatted text to facilitate easy reading and understanding of the analysis.

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

## Model Performance Summary

| Model                        | Train MSE        | Test MSE         | Train MAE  | Test MAE   | R² Score (Test) |
|------------------------------|------------------|------------------|------------|------------|-----------------|
| Linear Regression            | 83,885,896.98    | 84,636,829.12    | 6,941.06   | 6,963.16   | 0.4823          |
| Polynomial Degree 2          | 59,445,272.38    | 60,268,772.29    | 5,494.77   | 5,518.43   | 0.6314          |
| Polynomial Degree 3          | 49,857,795.67    | 50,789,617.50    | 4,894.22   | 4,925.46   | 0.6893          |
| Polynomial Degree 4          | 44,499,701.28    | 46,311,583.55    | 4,554.88   | 4,627.33   | 0.7167          |
| Lasso Regression (Degree 3)  | 49,862,361.33    | 50,786,715.52    | 4,893.22   | 4,924.48   | 0.6894          |
| Ridge Regression (Degree 3)  | 49,857,795.67    | 50,789,617.50    | 4,894.21   | 4,925.46   | 0.6893          |

## Recommendations

Focusing on the top attributes identified can significantly optimize dealership inventory management. These attributes include the year of the vehicle, odometer reading, drive type, cylinder count, fuel type, and transmission type. By prioritizing these factors, dealerships can enhance their inventory selection strategies to potentially maximize profitability.

However, a notable limitation of this model is its failure to account for expected profit and inventory turnover impacts. To provide a more comprehensive optimization strategy, additional data on profitability metrics and inventory turnover rates would be essential. For example, while vehicles with larger engines generally command higher prices, stocking vehicles with excessively high cylinder counts might limit potential market demand, potentially resulting in lower profits and revenue. Conversely, incentivizing sales of high-cylinder count vehicles could balance this effect by boosting demand.

Therefore, future exploration should focus on incorporating data that addresses these profitability and inventory turnover considerations. Additionally, exploring alternative modeling techniques such as logarithmic transformations could potentially improve inference accuracy beyond the standard polynomial of degree 3 model currently used.
