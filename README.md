# Hyponatremia Data Analysis and Modeling

This repository contains all the code, data, and documentation related to the preprocessing, modeling, and analysis of the MIMIC-IV dataset for hyponatremia. Below is a detailed description of the files and their contents.

## Files and Directories

### 1. `Preprocessing_mimiciv.ipynb`
   - **Description**: This Jupyter notebook contains the code for data preprocessing, cleaning, and merging various tables from the MIMIC-IV dataset.
   - **Data Files**: The preprocessing code works with the following data files, which are included in `data_files.zip`:
     - `prescriptions_filtered.csv`
     - `lab_events_filtered.csv`
     - `diagnoses_filtered.csv`
     - The final output of this preprocessing is `final_data.csv`, which is also included in `data_files.zip`.

### 2. `Catboost.ipynb`
   - **Description**: This notebook contains all the modeling code, including:
     - The implementation of the CatBoost model.
     - Hyperparameter tuning for CatBoost.
     - Performance evaluation of the CatBoost model.
     - Exploration and testing of other machine learning models.
     - Analysis of various caveats and challenges in the dataset.

### 3. `Catboost-component-wise.ipynb`
   - **Description**: This notebook extends the work done in `Catboost.ipynb` by applying the CatBoost model to two different patient clusters identified in the dataset.

### 4. `data_files.zip`
   - **Contents**:
     - `prescriptions_filtered.csv`
     - `lab_events_filtered.csv`
     - `diagnoses_filtered.csv`
     - `final_data.csv`

### 5. `ML hyponatremia treatment - final ppt.pptx`
   - **Description**: This file contains a comprehensive summary of the work, including data preprocessing, modeling, results, and conclusions.

## Instructions

1. **Preprocessing**:
   - Run the `Preprocessing_mimiciv.ipynb` notebook to preprocess and merge the MIMIC-IV tables into `final_data.csv`.

2. **Modeling**:
   - Use `Catboost.ipynb` to explore the dataset, run various models, and evaluate the performance of the final CatBoost model.
   - Run `Catboost-component-wise.ipynb` to apply the CatBoost model to the identified patient clusters.

3. **Review Summary**:
   - Refer to `ML hyponatremia treatment - final ppt.pptx` for an overview of the entire project, including key results and insights.

## Prerequisites

- Python 3.x
- Jupyter Notebook
- Libraries: `pandas`, `numpy`, `scikit-learn`, `catboost`, `matplotlib`, `seaborn`

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/hyponatremia_ml.git
