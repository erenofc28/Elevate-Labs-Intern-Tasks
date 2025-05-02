1️⃣ Load Dataset

The Iris dataset is loaded using load_iris().

2️⃣ Normalize Features

Data is standardized using StandardScaler() to improve distance-based calculations.

3️⃣ Split Data

The dataset is divided into training and testing sets using train_test_split().

4️⃣ Train KNN Model

A KNN classifier is initialized with n_neighbors=5 and trained on the dataset.

5️⃣ Make Predictions

The trained model predicts labels for the test set.

6️⃣ Evaluate Accuracy

The accuracy score is computed using accuracy_score(y_test, y_pred)
