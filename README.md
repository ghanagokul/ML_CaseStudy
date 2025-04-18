# ML_CaseStudy

## 🧠 Thought Process

I designed a two-stage machine learning pipeline to predict the likelihood of a user clicking a link in an email. The first model predicts whether the email will be clicked, and the second model focuses on link click prediction. I then developed a `recommend` function that evaluates all feature permutations based on a user's country and past purchase history, returning the combination with the highest final probability. To handle class imbalance, I applied the SMOTE technique, which was critical for improving model performance and ensuring fair predictions across classes.

## 🤔 Model Selection & Reasoning

I experimented with Random Forest, CatBoost, and Categorical Naive Bayes by categorizing the data. While Naive Bayes offered interpretability, the categorical data quality and encoding during testing posed challenges. Ultimately, I preferred Logistic Regression due to its simplicity and interpretability through coefficients, making it easier to explain and align with business understanding, despite being less complex than tree-based models.

