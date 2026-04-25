# Fintech-Credit-Portfolio-Optimization

## OverviewThe 
Fintech Risk Engine is an end-to-end analytical tool designed to process borrower datasets and provide predictive insights into financial risk. It transforms raw financial data into actionable intelligence through a pipeline of rigorous linear algebra operations and interactive visualizations.

## Technical Architecture
The system is built as a modular Python application, separating concerns between data architecture, mathematical processing, and the user interface:
* System Core (main.py): A custom Tkinter-based Graphical User Interface that manages the data pipeline, handles CSV uploads, and hosts real-time Matplotlib visualizations.
* Data Architect (1.py): Automates feature selection by applying the Rank-Nullity Theorem. It uses Reduced Row Echelon Form (RREF) to identify pivot columns and strip away linearly dependent (redundant) financial data.
* Mathematical Risk Engine (2.py): Performs the heavy lifting of risk prediction. It utilizes the Gram-Schmidt process to create an orthonormal basis of risk factors and solves the Least Squares problem (Ax = b) to generate predictive weights for borrower risk.
* System Optimization (3.py): Conducts Eigen-analysis on the covariance matrix of risk factors. This enables Principal Component Analysis (PCA) to cluster borrowers into distinct risk profiles based on primary and secondary risk trends.

## Core Features
Automated Redundancy Detection: Automatically detects if features like "Monthly Income" are simply linear derivatives of "Annual Income," removing them to prevent matrix singularity.

Interactive System Status Log: Provides real-time feedback on matrix rank, nullity, and pipeline execution status directly within the UI.

Professional Visualization Suite: Includes three primary analytical views:

Least Squares Prediction: Compares actual historical risk against model predictions.

Factor Independence: A heatmap displaying the success of Gram-Schmidt orthogonality.

Borrower Risk Clusters: A PCA-driven scatter plot identifying borrower intensity trends.

## Technology Stack
Languages: Python

Libraries: NumPy (Matrix Ops), SymPy (Symbolic Math/RREF), Pandas (Data Handling), Matplotlib/Seaborn (Visualization), Tkinter (GUI)

Mathematical Concepts: Orthogonalization, Eigen-decomposition, Rank-Nullity, Least Squares Regression

## Demo
<img width="1917" height="1008" alt="image" src="https://github.com/user-attachments/assets/2a81a230-77dd-477e-ac56-9f32380ad98e" />


<img width="1919" height="1006" alt="image" src="https://github.com/user-attachments/assets/c9a9240a-f32c-4acd-90da-ca7d26fa133a" />


<img width="545" height="257" alt="image" src="https://github.com/user-attachments/assets/b5893b52-ae6a-4a5f-a93b-8edae067ade7" />


