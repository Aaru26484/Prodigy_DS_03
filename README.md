\documentclass[12pt]{article}
\usepackage[a4paper, margin=1in]{geometry}
\usepackage{graphicx}
\usepackage{amsmath}
\usepackage{hyperref}
\usepackage{booktabs}
\usepackage{xcolor}
\usepackage{enumitem}

\title{\textbf{Bank Marketing Prediction using Decision Tree}}
\author{Task 3}
\date{\today}

\begin{document}

\maketitle

\section{Project Overview}
This project aims to predict whether a customer will subscribe to a bank term deposit using a Decision Tree Classifier. The dataset used is \texttt{bank-additional.csv}, and the target variable is \texttt{deposit} (renamed from \texttt{y}).

\section{Objectives}
\begin{itemize}
    \item Perform Exploratory Data Analysis (EDA)
    \item Preprocess the dataset
    \item Encode categorical features
    \item Train a Decision Tree model
    \item Evaluate model performance
    \item Visualize the Decision Tree
\end{itemize}

\section{Technologies Used}
\begin{itemize}
    \item Python
    \item Pandas
    \item NumPy
    \item Matplotlib
    \item Seaborn
    \item Scikit-learn
\end{itemize}

\section{Dataset Description}
\begin{itemize}
    \item Dataset Name: bank-additional.csv
    \item Separator: ;
    \item Target Variable: deposit
\end{itemize}

\section{Exploratory Data Analysis}
The following EDA techniques were applied:
\begin{itemize}
    \item Summary statistics using \texttt{describe()}
    \item Histograms for numerical features
    \item Count plots for categorical features
    \item Boxplots for outlier detection
    \item Correlation heatmap
\end{itemize}

\section{Data Preprocessing}
\begin{itemize}
    \item Removed highly correlated features: \texttt{cons.price.idx}, \texttt{cons.conf.idx}
    \item Label Encoding applied to categorical variables
    \item Features and target variable separated
\end{itemize}

\section{Model Training}
The dataset was split into training and testing sets:
\begin{itemize}
    \item Training: 70\%
    \item Testing: 30\%
\end{itemize}

The Decision Tree Classifier was trained using:
\begin{itemize}
    \item Criterion: Entropy
    \item Max Depth: 6
    \item Min Samples Split: 20
    \item Min Samples Leaf: 10
    \item Class Weight: Balanced
\end{itemize}

\section{Model Evaluation}
The model was evaluated using:
\begin{itemize}
    \item Accuracy Score
    \item Confusion Matrix
    \item Classification Report
\end{itemize}

Training and testing accuracies were compared to check for overfitting.

\section{Visualization}
The Decision Tree was visualized using the \texttt{plot\_tree()} function from Scikit-learn.

\section{How to Run the Project}
\begin{enumerate}
    \item Clone the repository.
    \item Install required libraries:
    \begin{verbatim}
    pip install pandas numpy matplotlib seaborn scikit-learn
    \end{verbatim}
    \item Run the Python script or Jupyter Notebook.
\end{enumerate}

\section{Conclusion}
This project demonstrates how a Decision Tree can be effectively used for classification tasks. Proper data preprocessing, EDA, and parameter tuning significantly improve model performance.

\end{document}
