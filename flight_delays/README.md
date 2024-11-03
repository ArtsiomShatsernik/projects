# Small educational project for the [Kaggle competition](https://www.kaggle.com/competitions/flight-delays-fall-2018).

**Objective:** predict whether a flight will be delayed for more than 15 minutes.

**Target metric:** ROC AUC.

# Project workflow:
* Exploratory Data Analysis with seaborn
* Feature engineering
  
<details>
    <summary>Details</summary>
<p></p>
Add about 15 new features. Most of which are related to departure time. This improved the metric by ~2.3 percent.

Potential new features:
- Distance related.
- Geographical: for example, the latitude and longitude of the origin cities or their average temperature.

---

</details>

* Feature selection
* Modeling with XGBoost
* XGB tuning with HyperOpt
* Modeling with Logistic Regression
* Logistic Regression tuning
* Using weighted averaging of XGBoost and Logistic Regression

<details>
  <summary>Details</summary>
<p></p>
It improved the result by about 0.03 percent.

XGBoost weight is 0.985, so it might be worth looking for a better linear model.

---

</details>

**Test Set ROC AUC:** 0.74119




