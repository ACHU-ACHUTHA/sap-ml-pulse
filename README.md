# SAP ML Pulse: Enterprise Customer Churn Predictor

## Overview
This project demonstrates an end-to-end machine learning pipeline that integrates directly with enterprise systems. By bridging Python's machine learning ecosystem with an SAP HANA database via the `hana_ml` library, this application extracts raw data, engineers predictive features, and trains a classification model to forecast customer behavior and potential churn.

## Tech Stack
* **Database:** SAP HANA Cloud
* **Data Processing:** Pandas, `hana_ml` (SAP Python Client)
* **Machine Learning:** `scikit-learn`
* **Environment:** Jupyter Notebooks

## Pipeline Architecture
The project is divided into a modular notebook pipeline:
1. **Database Connection:** Securely authenticating and connecting to the SAP HANA instance.
2. **Exploratory Data Analysis (EDA):** Leveraging HANA DataFrames to analyze data directly at the database level without massive local data extraction.
3. **Data Preprocessing:** Handling missing values, filtering high cardinality, and feature engineering.
4. **Model Training:** Splitting train/test data and applying classification algorithms.
5. **Hyperparameter Tuning:** Optimizing model performance for enterprise deployment.

## Installation & Setup
1. Clone this repository:
   ```bash
   git clone [https://github.com/ACHU-ACHUTHA/sap-ml-pulse.git](https://github.com/ACHU-ACHUTHA/sap-ml-pulse.git)
   Create and activate a virtual environment:

Bash
python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate
Install dependencies:

Bash
pip install -r requirements.txt
Launch the Jupyter server to run the pipeline:

Bash
jupyter notebook
Author
Developed by Achutha Kodamati


### 2. Files to Delete
The terminal output from your push shows a few files that instantly give away that this is an SAP CodeJam tutorial. Delete these files from your VS Code explorer:
*   `exercises/resources/SAPHANAMLCodeJam2503.pdf` (This is the instructor's slide deck).
*   `prerequisites.md` (This contains the workshop setup instructions).
*   The `exercises-selfstudy` folder (if it exists in your directory).

### 3. Rename the "Exercises" Folder
Having a folder named `exercises` makes it look like homework. 
*   Right-click the `exercises` folder in VS Code and rename it to **`notebooks`** or **`pipeline`**.

### 4. Clean Up the Markdown inside the Notebooks
Open the actual `.ipynb` files (like `010-check_setup.ipynb`). At the top of these files, there are usually Markdown blocks with text like *"Welcome to this CodeJam"* or *"Discuss with your instructor"*. 
*   Double-click those Markdown cells, delete the tutorial text, and replace it with a simple, professional heading (e.g., changing *"Exercise 1: Setting up your environment"* to just *"Step 1: Database Authentication"*).

Once you make these changes, save everything, commit the updates (`git add .`, `git commit -m "Refactor project structure and documentation"`), and push them to GitHub. 

<FollowUp label="Need help cleaning the notebooks?" query="Would you like me to provide exact replacement text for the markdown cells inside the first few Jupyter notebooks?"/>
