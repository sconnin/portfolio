---
date: 2021-11-19T11:13:32-04:00
description: "Logistic, Log-Normal, Gamma Models"
featured_image: "/images/insauc.jpg"
tags: []
title: "Insurance Classification and Prediction"
disable_share: false
---

This study sought to classify drivers based on their probability of an auto accident and to then predict the amount of claim payout associated with that accident. A synthetic data set of ~ 8000 observations was used to construct predictive models for this purpose. The use of synthetic data permitted model development absent proprietary information, while also providing a heuristic for quantitative reasoning.

{{< figure src="/images/insbivariate.jpg">}}

---
* Processed ~8000 observations for classification and predictive modeling.
* Engineered new features to improve model performance and to constrain uncertainties.
* Built and compared logistic classification models with varying thresholds. Final AUC=0.81.
* Constructed and compared log-normal and gamma models to predict claim payout.
* Identified issues with model fit and prospects for improvement based on prior studies.

---
Results

The covariates included in the dataset were sufficient to build/select an effective logistic classifier. Predicting claim payout proved more problematic - owing to the small number of covariates suited for individual payout predictions as well as lack of information on how payment amount was derived. A differentiated model based on binned values for the bluebook value of a vehicle may improve the accuracy of payment predictions.

---

[Rpubs - Report](https://rpubs.com/sconnin/856781)

[Github Repository](https://github.com/sconnin/insurance_model)
