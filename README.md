# Sale Price of House Case Study
---
## Case study assignment by IIIT Bangalore and Upgrad
---
> - Solving this assignment will give an idea of analysing the dataset and build a model to predict the variable of interest. Here, the interest is to predict the sale price of house based on few other parameters.
> - Developed as part of the Advanced Linear Regression Module required for Executive Post Graduate Program in Machine Learning and AI - IIIT,Bangalore.
---

## Table of Contents
* [General Information](#general-information)
* [Methodology](#methodology)
* [Repository contents](#repository-contents)
* [Conclusions](#conclusions)

## General Information
A US-based housing company named **Surprise Housing** has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia

**The company wants to know:**
- Which variables are significant in predicting the price of a house.
- How well those variables describe the price of a house.
  
**Objective:**
The company is looking at prospective properties to buy to enter the market. It is required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

## Methodology
1) Reading and Understanding the Data
2) Data manipulation and cleaning
3) Visualising the Data
4) Data Preparation
5) Splitting the Data into Training and Testing Sets
6) Building model

## Repository contents
| File | Description |
|:-----|:------------|
| Python notebook | It contains the complete detailed code along with necessary output to solve the problem|
| PDF | Answered the asked subjective questions. |
| README.md | This file briefs about the project. |
| train.csv | The sale price of house case study data set. |
| data definition.txt | Meaning of the variables in the dataset. |

## Conclusions
Metrics obtained using Ridge and Lasso regression models are:

| Metric |	Ridge Regression |	Lasso Regression |
|:-------|:------------------|:------------------|
| R2 Score (Train) |0.938550 |	0.931790 |
| R2 Score (Test) |	0.897946 |	0.910902 |
| RMSE (Train) |	0.032111 |	0.033831 |
| RMSE (Test)	| 0.040918 |	0.038232 |

- Since it is evident that both the models *R2 score* is same around **0.93** for train data and same around **0.90** for test data and *RMSE value* is same around **0.033** for train data and same around **0.038** for test data, it is better to select a model which is **simple**.
- In that terms, **lasso model** does better job since it does feature selection which resulted in *123 features* whereas ridge model has *298 features* which is 175 features more than lasso model.

Top features in *rank order* from **lasso** model are :
> - GrLivArea
> - OverallQual
> - Total_floor_SF
> - OverallCond
> - TotalBsmtSF
> - GarageArea
> - Neighborhood
> - Total_Bathrooms
> - LotArea
> - GarageCars
> - Fireplaces
> - Total_porch_sf
> - TotRmsAbvGrd
> - SaleType
> - Exterior1st_BrkFace
> - BsmtQual
> - Functional

Also, all the above features have a *positive correlation* with the Sale Price.

## Contact
Created by @shruthipv96 - feel free to contact me!
