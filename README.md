# Part 3: Regression-Based Business Insights & Model Interpretation

## Business Problem Summary

The objective of this project is to identify factors associated with monthly sales performance across retail stores and provide business recommendations using regression analysis.

Management wants to understand how variables such as marketing spend, customer traffic, inventory availability, and regional characteristics influence sales performance.

---

## Dataset Description

The dataset contains store-level business information including:

* Monthly Sales
* Marketing Spend
* Footfall
* Average Discount Percentage
* Staff Count
* Inventory Availability Percentage
* Competitor Distance
* Holiday Flag
* Customer Rating
* Region
* Store Type

---

## Dependent Variable

* monthly_sales

---

## Independent Variables

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* holiday_flag
* customer_rating
* region
* store_type

---

## Regression Approach

The analysis included:

1. Data cleaning and preparation
2. Creation of dummy variables for categorical data
3. Simple linear regression models
4. Multiple regression model
5. Residual analysis
6. Model comparison

---

## Dummy Variable Approach

Region was selected for dummy variable creation.

Reference Category:

* East

Dummy Variables:

* North
* South
* West

The East category was excluded to avoid multicollinearity and serve as the baseline category.

---

## Model Comparison Summary

| Model                  | R²    |
| ---------------------- | ----- |
| Marketing Spend        | 0.167 |
| Footfall               | 0.736 |
| Inventory Availability | 0.013 |
| Multiple Regression    | 0.811 |

The Multiple Regression Model achieved the highest explanatory power.

---

## Final Model Selected

Multiple Regression Model

Variables Included:

* marketing_spend
* footfall
* inventory_availability_pct
* region dummy variables

R² = 0.811

---

## Business Recommendation

The analysis indicates that footfall, marketing spend, and inventory availability are the strongest factors associated with monthly sales performance.

Management should prioritize strategies that increase customer traffic, maintain effective marketing investments, and improve inventory availability.

---

## Assumptions and Limitations

* Regression identifies association, not causation.
* Some important business factors may not be included in the dataset.
* External market conditions may affect sales performance.
* Regional effects may reflect additional local influences.

---

## Screenshots Included

* simple_regression_output.png
* multiple_regression_output.png
* residuals_preview.png
* model_comparison_preview.png

---

## Repository Structure

part3_regression_insights/

* data/
* analysis/
* outputs/
* screenshots/
* README.md

This repository contains all required files for Part 3: Regression-Based Business Insights & Model Interpretation.
