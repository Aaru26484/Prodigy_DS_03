\documentclass[12pt]{article}
\usepackage[a4paper, margin=1in]{geometry}
\usepackage{hyperref}
\usepackage{xcolor}

\title{\textbf{Bank Marketing Prediction using Decision Tree}}
\author{Task 3}
\date{\today}

\begin{document}

\maketitle

\section*{Abstract}
This project predicts whether a customer will subscribe to a bank term deposit using a Decision Tree Classifier. The dataset used is \texttt{bank-additional.csv}, and various data preprocessing, visualization, and machine learning techniques were applied.

\section*{Objectives}
\begin{itemize}
    \item Perform Exploratory Data Analysis (EDA)
    \item Preprocess the dataset
    \item Train a Decision Tree model
    \item Evaluate model performance
    \item Visualize the decision tree
\end{itemize}

\section*{Tools and Technologies}
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

\section*{Methodology}
The dataset was analyzed using descriptive statistics and visualizations. Categorical variables were encoded using Label Encoding. Highly correlated columns (\texttt{cons.price.idx}, \texttt{cons.conf.idx}) were removed. The dataset was split into 70\% training and 30\% testing data.

A Decision Tree Classifier was trained using entropy as the splitting criterion, with a maximum depth of 6, and class balancing applied.

\section*{Evaluation Metrics}
\begin{itemize}
    \item Accuracy Score
    \item Confusion Matrix
    \item Precision, Recall, and F1-score
\end{itemize}

\section*{Results}
The model achieved good classification performance on unseen data. Training and testing accuracies were compared to avoid overfitting.

\section*{Conclusion}
This project demonstrates that Decision Tree models are effective for classification problems when combined with proper preprocessing and EDA.

\end{document}
