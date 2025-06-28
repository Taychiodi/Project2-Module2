# Project2-Module2
This project investigates the causal impact of selling health supplements through iHerb versus other platforms like Amazon and Walmart, across different product categories and markets (USA, Canada, UK). Using data from IronKaggle and applying advanced causal inference techniques, we estimate the uplift or loss in revenue associated with iHerb.

## Dataset
Source: IronKaggle (provided by Ironhack)
Geographies covered: United States, Canada, United Kingdom
Observations: ~4,000 sales records
Main columns:
Date, Product Name, Category, Price, Revenue, Units Sold, Discount, Units Returned
Platform (iHerb, Amazon, Walmart)
Location (US, UK, Canada)


## Objectives:
Understand how platform choice (iHerb vs others) affects revenue
Explore heterogeneous effects by category and competition
Estimate treatment effect using causal machine learning
Deliver actionable insights via a dashboard in Tableau

## Models & Methodology
1. Feature Engineering
Created treatment variable: 1 if sold on iHerb, 0 otherwise
Computed competition as the number of unique products per Platform and Category
Added discount-adjusted revenue metrics and categorical encodings

2. Modeling Approaches
Model	Purpose
Random Forest	Baseline regression model for predicting revenue
Causal Forests	Estimated Conditional Average Treatment Effect (CATE)
Double ML (DML)	Estimated Average Treatment Effect (ATE) with confounder controls
Difference-in-Differences (DiD)	Compared pre/post revenue performance on iHerb vs control platforms

See full breakdown in the Tableau Dashboard

## Deliverables
Tableau Dashboard
Causal effect per category (bar chart)
Units Sold vs Units Returned (stacked bar with return % trendline)
Revenue vs Competition (scatter plot)
Filter by market, category, or platform

Ironhack Data Science and Machine Learning Bootcamp.

All analysis is educational and based on simulated sales data from IronKaggle.
