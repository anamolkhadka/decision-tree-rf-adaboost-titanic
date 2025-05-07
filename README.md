# 🌳 Decision Trees, Random Forests, and AdaBoost from Scratch

This project implements three core machine learning models from scratch in Python:

- **Decision Trees**  
- **Random Forests**  
- **AdaBoost (Boosting)**

The models are trained and evaluated on the classic **Titanic dataset** for binary survival prediction.  
The project deepens understanding of ensemble methods and tree-based classifiers without relying on high-level libraries like scikit-learn.

---

## 📚 Project Overview

### ✅ Models Implemented

- **DecisionTree**
  - Supports `gini`, `entropy`, and `misclassification` criteria
  - Handles `max_depth`, `min_samples_split`, `min_samples_leaf` hyperparameters
  - Recursive tree building and prediction

- **RandomForest**
  - Bootstrap sampling with replacement
  - Random feature subset selection per split
  - Aggregates predictions with majority voting

- **AdaBoost**
  - Uses DecisionTree as weak learners
  - Reweights misclassified samples iteratively
  - Combines learners using weighted sum of predictions

---

## 🛠 How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/tree-boosting-titanic.git
cd tree-boosting-titanic
```

2. Install dependencies:
```bash
pip install numpy pandas matplotlib seaborn
```

3. Use the provided dataset or Download the Titanic Dataset

### The Titanic Dataset

To test your implementations of the above algorithms, we use the Titanic dataset. This dataset contains passenger details and whether they survived the shipwreck.
The raw data needs preparation before use with the models.

Reference the popular notebook on Kaggle ["Introduction to Decision Trees (Titanic dataset)"](https://www.kaggle.com/code/dmilla/introduction-to-decision-trees-titanic-dataset)

You can download the data from the same page or use the provided dataset in the repository. Feel free to follow the preprocessing steps in the article or apply your own feature engineering.

4. Run the Jupiter notebook:
```bash
jupyter notebook trees_and_boosting.ipynb
```


## ✨ Dataset Preprocessing
- Dropped irrelevant features (e.g., Name, Ticket, Cabin)
- Filled missing values (e.g., Age, Embarked)
- Converted categorical variables to numerical (Sex, Embarked)
- Normalized or standardized relevant numerical features


## 💡 Features & Highlights
- Handcrafted decision tree splitting and stopping rules
- Bagging and feature randomness for ensemble diversity in Random Forests
- Adaptive boosting with weight updates on misclassified samples
- Evaluation on Titanic dataset with clear result tables and visualizations


## 📊 Evaluation Summary
Model	        Accuracy (Test Set)
Decision Tree	79%
Random Forest	83%
AdaBoost	    85%

✅ AdaBoost achieved the highest accuracy on the Titanic dataset.


## 🎓 Key Learnings
- Understanding impurity measures and splitting criteria
- How bootstrap aggregation reduces variance
- How boosting reduces bias by focusing on hard-to-classify examples
- Importance of data cleaning and feature selection in real-world datasets


## 📚 References

- [Kevin P. Murphy, *Probabilistic Machine Learning: An Introduction*](https://probml.github.io/pml-book/book1.html)
- [Leo Breiman, *Random Forests* (2001)](https://www.stat.berkeley.edu/~breiman/randomforest2001.pdf)
- ["Introduction to Decision Trees (Titanic dataset)"](https://www.kaggle.com/code/dmilla/introduction-to-decision-trees-titanic-dataset)


## 📜 License

- © 2025 **Anamol Khadka**. All rights reserved.
- This work is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.
- You are free to **share** and **adapt** the material for any purpose, even commercially, as long as **appropriate credit** is given.
- Unauthorized reproduction, distribution, or modification of this work **without attribution** is prohibited.
- For permissions or inquiries, please contact: [khadkaanamol8@gmail.com](mailto:khadkaanamol8@gmail.com)

