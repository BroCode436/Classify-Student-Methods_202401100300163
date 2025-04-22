# Student Learning Style Classification and Clustering

This project focuses on classifying students based on their learning styles (Visual, Auditory, Kinesthetic) by analyzing scores in these categories. Additionally, it clusters students based on their learning style preferences using KMeans clustering. The project also evaluates the classification results by using confusion matrices and various performance metrics, such as accuracy, precision, and recall.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Objectives](#objectives)
3. [Methodology](#methodology)
4. [Installation and Setup](#installation-and-setup)
5. [Usage](#usage)
6. [Visualizations](#visualizations)
7. [Evaluation Metrics](#evaluation-metrics)
8. [References](#references)

## Project Overview

The project utilizes a dataset containing students' scores in three learning methods—visual, auditory, and kinesthetic—to predict their dominant learning style. It performs classification by selecting the highest score for each student to predict their learning style. The project also includes clustering to group students based on their score similarities, with the aim of uncovering underlying patterns in learning preferences.

### Key Features:
- **Learning Style Classification**: Assign students to one of three learning styles based on their score inputs.
- **KMeans Clustering**: Group students into clusters based on their learning scores.
- **Confusion Matrix Heatmap**: Visualize the effectiveness of the classification using a heatmap.
- **Performance Evaluation**: Calculate and display accuracy, precision, and recall to assess the classification results.

## Objectives

The primary objectives of this project are:
1. **To classify students** into one of the three learning styles based on their performance in visual, auditory, and kinesthetic categories.
2. **To evaluate the accuracy of the classification model** by comparing the predicted learning styles with the actual learning styles.
3. **To apply clustering techniques** like KMeans to identify potential groups of students with similar learning styles.
4. **To visualize results** through bar charts, pie charts, and confusion matrix heatmaps.
5. **To calculate key evaluation metrics** (accuracy, precision, recall) for model evaluation.

## Methodology

### 1. **Data Collection**
   The dataset, `student_methods.csv`, includes the following columns:
   - `visual_score`: Score representing the visual learning style.
   - `auditory_score`: Score representing the auditory learning style.
   - `kinesthetic_score`: Score representing the kinesthetic learning style.
   - `learning_style`: The actual learning style of the student (used for evaluation).

### 2. **Classification**
   The learning style for each student is predicted by selecting the highest score among the three (visual, auditory, and kinesthetic). This is achieved by:
   - Using a custom function to assign the dominant learning style based on the highest score.

### 3. **Clustering**
   KMeans clustering is applied to group students based on their scores. This helps uncover patterns and similarities in the students' learning preferences.

### 4. **Visualization**
   The following visualizations are used to understand the data better:
   - **Bar Chart**: Displays the distribution of students across the three learning styles.
   - **Pie Chart**: Shows the percentage of students in each learning style.
   - **Confusion Matrix Heatmap**: A heatmap to visualize the comparison between actual and predicted learning styles.

### 5. **Evaluation Metrics**
   Key performance metrics used to evaluate the classification model include:
   - **Accuracy**: The percentage of correct predictions.
   - **Precision**: The weighted average of precision across all classes.
   - **Recall**: The weighted average of recall across all classes.

## Installation and Setup

### Requirements

- **Python 3.x**
- **Libraries**: Pandas, Matplotlib, Seaborn, Scikit-learn, NumPy

You can install all dependencies using `pip`:

```bash
pip install pandas matplotlib seaborn scikit-learn numpy
