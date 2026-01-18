📊 Prodigy Infotech – Data Science Internship
Task 03: Decision Tree Classification
👤 Intern

Aarti Singh

📌 Task Description

The objective of this task is to build a Decision Tree Classifier to predict whether a customer will subscribe to a bank term deposit. The task includes data preprocessing, EDA, feature encoding, model training, evaluation, and visualization.

🎯 Objectives

Load and inspect the dataset

Perform EDA

Encode categorical variables

Train a Decision Tree model

Evaluate model performance

Visualize the Decision Tree

📂 Dataset

Dataset Used: Bank Marketing Dataset (bank-additional.csv)

Contains customer details such as age, job, education, marital status, etc.

Target Variable: deposit

🛠️ Tools & Technologies

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab / Jupyter Notebook

🔍 Exploratory Data Analysis

Steps performed:

Data loading and inspection

Missing & duplicate value check

Numerical & categorical feature analysis

Data visualization

Correlation analysis

📈 Correlation Heatmap
df_dummies = pd.get_dummies(df)
corr = df_dummies.corr()

plt.figure(figsize=(12,8))
sns.heatmap(corr, cmap='coolwarm')
plt.show()

⚙️ Data Preprocessing

Removed highly correlated columns

Label Encoding applied

Train-test split (70%–30%)

🌳 Model Training
dt = DecisionTreeClassifier(
    criterion='entropy',
    max_depth=6,
    min_samples_split=20,
    min_samples_leaf=10,
    class_weight='balanced'
)

📊 Model Evaluation
print("Accuracy:", accuracy_score(y_test, y_pred))
print(confusion_matrix(y_test, y_pred))
print(classification_report(y_test, y_pred))

🌿 Decision Tree Visualization
plt.figure(figsize=(30,20))
plot_tree(
    dt,
    feature_names=X.columns,
    class_names=['No','Yes'],
    filled=True,
    fontsize=10
)
plt.show()

✅ Conclusion

This task demonstrates the effectiveness of Decision Tree classifiers in solving classification problems through proper preprocessing, EDA, and model tuning.

If you want, I can now:

✅ Put this into a README.md file
✅ Make it 1-page
✅ Convert to PDF
✅ Add screenshots

Just say the word 😎
