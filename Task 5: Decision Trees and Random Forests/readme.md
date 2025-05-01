Step 1: Load & Split Dataset
Uses the Breast Cancer dataset from Scikit-learn.

Splits the data into training and testing sets for model evaluation.

Step 2: Train & Visualize Decision Tree
Builds a DecisionTreeClassifier with max_depth=4 to control overfitting.

Uses Matplotlib to visualize the tree structure.

Step 3: Train Random Forest & Compare Accuracy
Implements a RandomForestClassifier with n_estimators=100.

Measures model accuracy on the test set.

Step 4: Analyze Feature Importance
Extracts feature importance from Random Forest.

Sorts & displays the most influential features.

Step 5: Evaluate Model Using Cross-Validation
Performs 5-fold cross-validation
