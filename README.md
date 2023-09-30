# ADABOOST_ML

AdaBoost (Adaptive Boosting) is an ensemble learning algorithm that combines the predictions of multiple base estimators (usually decision trees) to improve overall predictive performance.

It focuses on learning from the mistakes of the weak learners and assigns more weight to misclassified samples.

**How AdaBoost works:**

**1. Initialization:**
-  All data points are given equal weight.

**2. Iteration:**

- **Fit a Weak Learner:** Train a weak learner (typically a decision tree with a small depth) on the data. The weak learner's performance is only slightly better than random guessing.

- **Compute Error:** Calculate the error rate of the weak learner. This is the proportion of misclassified samples.

- **Compute Weight:** Assign a weight to the weak learner based on its error rate. A lower error rate leads to a higher weight.

- **Update Weights:** Adjust the weights of the misclassified samples. Misclassified samples are given higher weight so that they are more likely to be correctly classified in the next iteration.

- **Combine Predictions:** Combine the predictions of all weak learners. Stronger emphasis is given to the predictions of the weak learners with higher weights.

- **Final Prediction:** The final prediction is made by summing up the weighted predictions.

**Advantages of AdaBoost:**

**1. High Accuracy:** 
- AdaBoost is known for its high accuracy and is less prone to overfitting compared to individual weak learners.

**2. Versatility:**
- It can be used with a variety of base estimators, not just decision trees.

**3. Handles Both Classification and Regression:**
- AdaBoost can be used for both classification and regression tasks.

**4. Feature Importance:**
- AdaBoost provides a way to calculate feature importance, which can be useful for understanding which features are contributing the most to the model's predictions.



**Disadvantages of AdaBoost:**

**1. Sensitivity to Noisy Data and Outliers:** 
- AdaBoost can be sensitive to noisy data and outliers. It may try to fit the noisy data, leading to overfitting.

**2. Computationally Intensive:** 
- It can be computationally intensive, especially when using a large number of weak learners or complex base estimators.

**3. Less Interpretable:**
- The final model produced by AdaBoost can be less interpretable compared to a single decision tree.

**4. Requires Sufficient Data:**
- AdaBoost may not perform well on very small datasets or datasets with high noise.

**5. Less Control Over Individual Weak Learners:**
- AdaBoost does not allow much control over the individual weak learners. It focuses on improving the ensemble's performance as a whole.
