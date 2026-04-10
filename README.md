# Heart Disease Classification 🩺

This project uses Machine Learning to predict whether a patient has heart disease based on their medical attributes. By analyzing clinical data, we developed a model capable of assisting in medical diagnosis with high accuracy.

## 📊 Project Overview & Results
I experimented with three different machine learning models to find the most reliable predictor. After comparing their baseline performance and tuning their hyperparameters, the results were:

* **Logistic Regression:** **88% Accuracy** (Best Performer 🏆)
* **K-Nearest Neighbors (KNN):** 68%
* **Random Forest Classifier:** 86%

**Logistic Regression** was the most effective model for this dataset, providing the best balance between precision and recall.

## 🛠️ Tools and Libraries
* **Python** - Core language
* **Pandas** - Data manipulation
* **NumPy** - Numerical operations
* **Scikit-Learn** - Model development, hyperparameter tuning (`GridSearchCV`, `RandomizedSearchCV`), and evaluation metrics.
* **Matplotlib & Seaborn** - Data visualization and correlation heatmaps.

## 🔍 Workflow
1. **Exploratory Data Analysis (EDA):** Visualized the data to find patterns. Used a **Correlation Matrix (Heatmap)** to identify which features (like `cp` - chest pain and `thalach` - max heart rate) had the strongest impact on the target.
2. **Data Splitting:** Divided the data into training (80%) and test (20%) sets to ensure the model generalizes well to new data.
3. **Hyperparameter Tuning:** * Used `RandomizedSearchCV` for quick exploration of the parameter space.
    * Used `GridSearchCV` for fine-tuning the `C` parameter in Logistic Regression.
4. **Model Evaluation:** Evaluated the "Winning" model using:
    * **Confusion Matrix:** To see where the model made false positive vs. false negative errors.
    * **ROC Curve & AUC:** To measure the trade-off between sensitivity and specificity.
    * **Classification Report:** Detailed Precision, Recall, and F1-score.

## 🚀 Installation & Usage
To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/heart-disease-project.git](https://github.com/YOUR_USERNAME/heart-disease-project.git)

2. **Create a virtual environment:**
   ```bash
   python -m venv env

4. **Activate the environment:**
   ```bash
   Windows: .\env\Scripts\activate
   Mac/Linux: source env/bin/activate

6. **Install the required libraries:**
   ```bash
   pip install -r requirements.txt

8. **Launch Jupyter Notebook:**
   jupyter notebook

## 📈 Conclusion
The high accuracy of 88% achieved by the Logistic Regression model suggests that the relationship between these clinical features is relatively linear. This project serves as a strong foundation for medical binary classification tasks.
