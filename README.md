# Social Network Ads Purchase Prediction Using Decision Tree Classification

## Project Overview

This project is a Machine Learning classification project developed to predict whether a user will purchase a product after viewing a social network advertisement.

The project uses a Decision Tree Classification model and follows a complete Machine Learning workflow, including:

- Dataset loading and exploration
- Categorical feature encoding
- Feature selection
- Train-test splitting
- Model training
- Model evaluation
- Model serialization
- Prediction using new user input

The project contains a training notebook and a separate deployment notebook for loading the saved model and making predictions.

---

## Project Structure

```text
Social-Network-Ads-Decision-Tree/
│
├── 01.Decision_Tree_Social_Networks_Ads_Prediction(1).ipynb
├── 02_Decision_Tree_Model_Deployment.ipynb
├── Social_Network_Ads(2).csv
├── Finalized_model (1)(3).sav
└── README.md
```

---

## Technologies Used

| Category | Technology |
|---|---|
| Programming Language | Python |
| Data Analysis | Pandas |
| Data Visualization | Matplotlib |
| Statistical Visualization | Seaborn |
| Machine Learning | Scikit-learn |
| Classification Algorithm | Decision Tree Classifier |
| Model Serialization | Pickle |

---

## Dataset Information

The project uses the Social Network Ads dataset.

The dataset contains user information related to social network advertising and a target indicating whether the user purchased the product.

### Dataset Features

| Feature | Description |
|---|---|
| User ID | Unique identifier for a user |
| Gender | Gender of the user |
| Age | Age of the user |
| EstimatedSalary | Estimated salary of the user |
| Purchased | Target indicating whether the product was purchased |

### Target Variable

```text
Purchased
```

The target represents two possible classes:

```text
0 = Not Purchased
1 = Purchased
```

---

## Machine Learning Workflow

### 1. Dataset Loading

The dataset is loaded using Pandas and inspected to understand its structure, columns, and values.

---

### 2. Data Preprocessing

The categorical `Gender` feature is converted into numerical representation so that it can be used by the Machine Learning model.

The encoded data is prepared for model training by selecting the relevant input features.

---

### 3. Feature Selection

The model uses the customer information required for purchase prediction.

The primary input variables are:

```text
Age
EstimatedSalary
Gender
```

The target variable is:

```text
Purchased
```

---

## Train-Test Split

The dataset is divided into training and testing subsets.

The training data is used to learn the decision rules, while the testing data is used to evaluate the model on unseen observations.

---

## Decision Tree Classification

The project uses:

```python
DecisionTreeClassifier
```

A Decision Tree Classifier predicts a class by learning a sequence of decision rules from the training data.

For this project, the classifier determines whether a user is likely to:

```text
Purchase
```

or:

```text
Not Purchase
```

---

## Model Training

The Decision Tree model is trained using the prepared training features and target values.

The trained classifier can then generate predictions for the test dataset and new user inputs.

---

## Model Evaluation

The project evaluates the classification model using classification-oriented evaluation techniques.

The evaluation workflow compares the actual target values with the model's predicted values.

Typical outputs in the project include classification performance analysis and visual representation of the prediction results where included in the notebook.

---

## Data Visualization

The project uses Python visualization libraries to explore the dataset and understand relationships between the input variables and purchase behavior.

The visual analysis helps provide a better understanding of the distribution and patterns present in the Social Network Ads dataset.

---

## Model Serialization

After training, the Decision Tree model is saved as a Pickle file:

```text
Finalized_model (1)(3).sav
```

Saving the trained model allows it to be loaded later without repeating the complete training process.

---

## Model Deployment Workflow

The deployment notebook demonstrates how the saved Decision Tree model can be loaded and used for prediction.

The workflow is:

```text
Load Saved Model
       |
       v
Receive New User Input
       |
       v
Prepare Input Features
       |
       v
Generate Prediction
       |
       v
Display Purchase Result
```

The deployment process uses the same feature structure required by the trained model.

---

## Example Prediction

A new user's information can be supplied using:

```text
Age
Estimated Salary
Gender
```

The model processes the input and produces a binary classification:

```text
0 = Not Purchased
1 = Purchased
```

The prediction can then be presented as a readable purchase decision.

---

## Project Workflow Summary

```text
Social Network Ads Dataset
          |
          v
    Data Exploration
          |
          v
   Data Preprocessing
          |
          v
   Gender Encoding
          |
          v
   Feature Selection
          |
          v
    Train-Test Split
          |
          v
 Decision Tree Classifier
          |
          v
      Prediction
          |
          v
     Evaluation
          |
          v
   Model Serialization
          |
          v
    New User Input
          |
          v
 Purchase Prediction
```

---

## Learning Outcomes

This project demonstrates practical understanding of:

- Supervised Machine Learning
- Binary classification
- Decision Tree Classification
- Feature selection
- Categorical variable encoding
- Train-test splitting
- Model prediction
- Classification model evaluation
- Data visualization
- Model serialization using Pickle
- Applying a trained model to new data

---

## Future Improvements

Potential improvements for this project include:

- Hyperparameter tuning
- Cross-validation
- Feature scaling comparison
- Decision Tree visualization
- Feature importance analysis
- ROC-AUC evaluation
- Precision and recall analysis
- Comparison with Logistic Regression, SVC, KNN, Random Forest, and Naive Bayes
- Streamlit-based interactive deployment
- Cloud deployment

---

## Author

**MANIKANDAPRABHU.S**

Machine Learning and Artificial Intelligence Enthusiast

---

## License

This project is intended for educational and learning purposes.
