# Breast_Cancer-Classification

#### The goal of this project was to evaluate the performance of five supervised learning algorithms on the breast cancer dataset from the sklearn library. The dataset contains information about various features of breast tumors, categorized as either benign or malignant. Our focus was on identifying the best-performing model based on accuracy.

### 1. Logistic Regression
How it Works: Logistic Regression is a linear model used for binary classification. It predicts the probability of a class (e.g., benign or malignant) using the sigmoid function to map linear outputs to probabilities between 0 and 1. The decision boundary is determined by a threshold (usually 0.5). Works well for linearly separable data. It Provides interpretable results, especially for binary classification problems like this one.
#### Logistic Regression ahieved high accuracy 0.95

### 2.Decision Tree Classifier
How it Works: Decision Trees split the dataset into subsets based on feature values, creating a tree structure. At each node, the algorithm selects the feature that provides the best split using metrics like Gini impurity or entropy. This continues until leaf nodes represent classes. Easy to interpret and visualize. It handles both numerical and categorical data.
However, prone to overfitting, which can limit performance.
#### Decision Tree Classifier achieved high accuracy of 0.93
##### The Decision Tree performed the worst because it is prone to overfitting, especially on smaller datasets. Unlike Random Forest, it lacks the ensemble feature to counterbalance this issue.

### 3. Random Forest Classifier
Random Forest is an ensemble learning algorithm that combines the predictions of multiple decision trees. It trains each tree on a random subset of features and data points, and aggregates their predictions (via majority voting for classification). Reduces overfitting compared to a single Decision Tree. It Robust to noise and works well with high-dimensional datasets.It Can handle complex interactions between features.
#### achieved high accuracy of 0.97
##### Reason: Random Forest, an ensemble learning technique, combines predictions from multiple decision trees to reduce overfitting and improve generalization. It excels in handling high-dimensional datasets like this one, providing robust results even with noise or irrelevant features.

### 4. Support Vector Machine (SVM)
How it Works: SVM finds the hyperplane that best separates data points into classes. It maximizes the margin (distance) between the hyperplane and the nearest data points (support vectors). It can also handle non-linear data using kernel tricks (e.g., RBF kernel). Effective for datasets that are not perfectly linearly separable. Works well with high-dimensional spaces, which is important for datasets with many features.
#### Support Vector Machine (SVM) achieved high accuracy of 0.96. 
##### These models are well-suited for binary classification tasks where the dataset is linearly separable.

### k-Nearest Neighbors (k-NN)
Accuracy: 0.94
k-NN is a non-parametric algorithm that classifies a data point based on the majority class of its k nearest neighbors in the feature space. The distance metric (e.g., Euclidean) is used to identify the nearest neighbors.
## Conclusion
Based on the results:
The Random Forest Classifier is the most suitable model for this dataset due to its high accuracy and robustness.
The Decision Tree Classifier performed the worst, highlighting the importance of using ensemble methods to improve prediction accuracy.
