# Sleep Health and Lifestyle Predictive Modeling

This repository contains a project focused on analyzing and predicting key factors related to sleep health and lifestyle, using the **Sleep Health and Lifestyle Dataset**. The goal is to explore the data, perform feature engineering, and build a predictive model to forecast sleep quality based on various health and lifestyle factors.

## Dataset

The dataset includes the following columns:

- **Person ID**: An identifier for each individual.
- **Gender**: The gender of the person (Male/Female).
- **Age**: The age of the person in years.
- **Occupation**: The occupation or profession of the person.
- **Sleep Duration (hours)**: The number of hours the person sleeps per day.
- **Quality of Sleep (scale: 1-10)**: A subjective rating of the quality of sleep, ranging from 1 to 10.
- **Physical Activity Level (minutes/day)**: The number of minutes the person engages in physical activity daily.
- **Stress Level (scale: 1-10)**: A subjective rating of the stress level experienced by the person, ranging from 1 to 10.
- **BMI Category**: The BMI category of the person (e.g., Underweight, Normal, Overweight).
- **Blood Pressure (systolic/diastolic)**: The blood pressure measurement of the person, indicated as systolic pressure over diastolic pressure.
- **Heart Rate (bpm)**: The resting heart rate of the person in beats per minute.
- **Daily Steps**: The number of steps the person takes per day.
- **Sleep Disorder**: The presence or absence of a sleep disorder in the person (None, Insomnia, Sleep Apnea).

## Project Overview

### 1. **Data Exploration**
Data exploration involves understanding the structure, distributions, and relationships of the dataset. Key steps include:
- Cleaning the data (handling missing values, correcting column names, etc.).
- Visualizing the distributions of numerical and categorical features.
- Performing correlation analysis to identify relationships between variables.

### 2. **Feature Engineering**
We perform necessary transformations, such as:
- Converting `Blood Pressure` into two separate columns: **HighBP** and **LowBP** (systolic and diastolic values).
- Adjusting the `BMI Category` column to replace "Normal Weight" with "Normal".
- Creating features for outlier detection and handling.

### 3. **Outlier Detection**
Outliers are detected and visualized using **boxplots**, which help identify extreme values in the dataset that could affect model performance. The boxplot method helps to visually identify potential outliers for further examination.

### 4. **Predictive Modeling**
Using machine learning algorithms, we aim to predict **Quality of Sleep** based on the various features. Key steps include:
- Preprocessing the data.
- Selecting appropriate models (e.g., Random Forest, Gradient Boosting).
- Evaluating model performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.

### 5. **Model Evaluation**
We evaluate the predictive model using common metrics:
- **MAE (Mean Absolute Error)**: Measures the average magnitude of the errors in predictions.
- **MSE (Mean Squared Error)**: Provides a quadratic penalty for larger errors.
- **R² Score**: Measures the proportion of variance explained by the model.

## Technologies Used

- **Python 3.x**
- **Libraries**: pandas, numpy, seaborn, matplotlib, scikit-learn
- **Jupyter Notebooks** for exploratory data analysis and modeling

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/yourusername/sleep-health-predictive-modeling.git
    ```

2. Navigate to the project directory:

    ```bash
    cd sleep-health-predictive-modeling
    ```

3. Install required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Run Jupyter Notebook:

    ```bash
    jupyter notebook
    ```

## How to Use

1. **Data Exploration**: Begin by running the data exploration script to understand the dataset. This includes visualizations of feature distributions and correlation analysis.
2. **Feature Engineering**: After exploring the data, proceed to clean and prepare the dataset for modeling, such as splitting the `Blood Pressure` column and adjusting the `BMI Category`.
3. **Outlier Detection**: Use the boxplots to detect and address outliers.
4. **Build Predictive Models**: Select and train machine learning models to predict **Quality of Sleep**. Evaluate their performance and choose the best model.
5. **Model Evaluation**: Review the evaluation metrics and finalize the model.

## Example Usage

Run the notebook or script for data exploration and predictive modeling:

```bash
python data_exploration.py
python predictive_modeling.py