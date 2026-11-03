# Final Conclusion

In this practical session, we explored different hypothesis spaces, feature representations, and regression models to understand their impact on predictive performance and generalization.

We started by exploring the dataset, which contains 10 observations representing students' study hours and exam scores. We visualized the relationship between the two variables and examined the dataset using descriptive statistics.

In **Part A**, we trained and compared six models: Linear Regression, Polynomial Regression (degrees 2 and 3), Decision Trees (depths 1 and 3), and K-Nearest Neighbors (k=3). We evaluated their training performance using RMSE and R² and visualized their predictions.

In **Part B**, we introduced Leave-One-Out Cross-Validation (LOOCV) to evaluate model generalization. We tested polynomial degrees 1, 2, 3, 5, and 9, comparing training RMSE with LOOCV RMSE. The results highlighted the importance of model complexity and the risk of overfitting.

In **Part C**, we investigated different feature representations and regularization techniques. The original representation using only \(x\) achieved the best LOOCV RMSE of **1.548637**, compared with 2.061987 for degree 3 and 3.706962 for degree 5.

We then evaluated Ridge and Lasso using degree-5 polynomial features and different alpha values. The best regularized configuration was **Lasso with alpha = 0.1**, achieving a LOOCV RMSE of **1.622286**. Regularization significantly improved the degree-5 polynomial model, reducing its LOOCV RMSE from 3.706962 to 1.622286.

Finally, in **Part D**, we selected the best configuration from each model family and performed a final comparison using Training RMSE and LOOCV RMSE.

The best overall model was **Linear Regression (degree 1)**, with:
- Training RMSE: **1.167229**
- LOOCV RMSE: **1.548637**

The results demonstrate that increasing model complexity does not necessarily improve generalization. More complex models may achieve lower training errors while performing worse on unseen observations. Regularization can help control overfitting, but a simpler model may still provide better predictive performance.

Overall, this practical session demonstrates the importance of feature representation, model selection, cross-validation, and regularization in building models that generalize well. However, since the dataset contains only 10 observations, the results should be interpreted cautiously and further validated using a larger dataset.
