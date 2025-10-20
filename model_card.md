# Model Card

## 

## Model Description

**Model Architecture:**

* Linear and Ridge regression - Linear models mapping predictors to paid loss values with Ridge included for stability.
* Random Forest: A collection of decision trees built on different random samples of the data, with their predictions averaged to smooth out noise and reduce overfitting.
* Gradient Boosting: Builds many small trees in sequence, where each new tree focuses on fixing the mistakes made by the previous ones.
* Bayesian Optimization: A smarter way of searching for the best settings (like tree depth, number of trees, or learning rate) by learning from past trials instead of testing parameters at random.



**Inputs:**

* **Calendar/triangle indices:** Accident year, development year\*\*.\*\*
* **Exposure measures:** Premiums or earned exposure.
* **Claims aggregates:** Incurred losses, bulk reserves, or similar summary fields.
* **Preprocessed tabular data:** Cleaned, split into training and test sets.



**Output:**

* Predicted cumulative paid loss for each observation in the test set
* Evaluation metrics: RMSE, MAE, and R2(Squared) to assess accuracy.

## Performance

&nbsp;                               Model          RMSE          MAE        R²

0                   Linear Regression  78156.396157  6663.416690  0.945363

1                    Ridge Regression  78156.396157  6663.416690  0.945363

2                       Random Forest  57383.111518  4168.973760  0.970547

3                   Gradient Boosting  56603.408984  3959.675173  0.971342

4      Tuned Random Forest (Bayesian)  60498.962170  4193.203106  0.967262

5  Tuned Gradient Boosting (Bayesian)  56925.553179  3897.913599  0.971015



Gradient Boosting and tuned Gradient boosting were the best performing models as they had the lowest RMSE, MAE and highest R2 (squared)

The linear models captured the trend well however they had more margin for error.

Therefore implying that are other factors at play when it comes to the relationship between earned premium and actual claims.



## Limitations

The model relies heavily on consistent historical patterns, this implies that it may not work well if new factors come into play such as new premium pricing methods that can improve the premium earning for the insurers. In order to mitigate this, we should use scenario testing and judgment when deciding to allocate capital to a line of business.

## Trade-offs

Linear models give the most accurate and straightforward results, but they could miss factor if the data becomes more complex in the future. Tree‑based models are better at handling those kinds of shifts.

However in this model, they are less accurate and more difficult to manage and explain.

