\documentclass[12pt]{article}
\usepackage[a4paper, margin=1in]{geometry}
\usepackage{graphicx}
\usepackage{xcolor}
\usepackage{hyperref}
\usepackage{listings}
\usepackage{titlesec}

\title{\textbf{Prodigy Infotech – Data Science Internship}\\
\large Task 02: Data Cleaning \& Exploratory Data Analysis (EDA)}
\author{\textbf{Intern: Aarti Singh}}
\date{\today}

\begin{document}

\maketitle

\section*{Task Description}
The objective of this task is to perform \textbf{data cleaning} and \textbf{exploratory data analysis (EDA)}
on a dataset in order to understand its structure, explore relationships between variables,
and extract meaningful insights before applying machine learning techniques.

\section*{Objectives}
\begin{itemize}
    \item Clean and preprocess the dataset
    \item Handle missing and inconsistent values
    \item Analyze numerical features
    \item Identify correlations between variables
    \item Visualize data using plots and heatmaps
\end{itemize}

\section*{Dataset}
\begin{itemize}
    \item \textbf{Dataset Used:} Titanic Dataset
    \item The dataset contains passenger information such as age, fare, class, and survival status.
\end{itemize}

\section*{Tools \& Technologies}
\begin{itemize}
    \item Python
    \item Pandas
    \item NumPy
    \item Matplotlib
    \item Seaborn
    \item Google Colab / Jupyter Notebook
\end{itemize}

\section*{Exploratory Data Analysis}
The following steps were performed:
\begin{enumerate}
    \item Data loading and inspection
    \item Handling missing values
    \item Selection of numerical features
    \item Correlation analysis
    \item Visualization using a correlation heatmap
\end{enumerate}

\section*{Correlation Heatmap}
The correlation heatmap below visualizes relationships between numerical features in the dataset:

\begin{lstlisting}[language=Python]
plt.figure(figsize=(8,6))

numeric_df = df.select_dtypes(include=['int64', 'float64'])
sns.heatmap(numeric_df.corr(), annot=True, cmap='coolwarm')

plt.title("Correlation Heatmap (Numeric Features)")
plt.show()
\end{lstlisting}

\end{document}
