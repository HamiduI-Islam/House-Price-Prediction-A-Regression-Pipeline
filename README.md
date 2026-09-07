# 🏠 House Price Estimation and Regression Pipeline

A rigorous, leakage-free machine learning pipeline built to predict residential real estate prices using physical and locational attributes. This project follows a strict 11-step data science workflow, comparing a baseline predictor against Linear Regression and Random Forest models.

---

## 📁 File Structure

To satisfy the execution requirements, our project uses the following centralized file structure:

*   `housing.csv`: The raw dataset (unmodified source file).
*   `notebook.ipynb`: Our complete, executable Jupyter/Colab notebook.
*   `requirements.txt`: A record of Python and package dependencies to recreate our environment.
*   `README.md`: Project documentation and setup instructions.

---

## 🛠️ Environment Setup & Dependencies

To ensure a reviewer can recreate our main tables, figures, and metrics, we have provided our package versions in the environment file. 

**Setup Instructions:**
1. Clone the repository to your local machine.
2. Install the required dependencies via the command line:
   `pip install -r requirements.txt`

---

## 📊 Data Access & Placement

*   **Data Source:** The `housing.csv` dataset is publicly sourced from Kaggle real estate repositories.
*   **Data Placement:** Please ensure `housing.csv` is placed directly in the root directory alongside `notebook.ipynb`. 
*   **Raw State:** We have maintained an unchanged raw copy of the dataset; no manual edits were made without documenting the rule in our code[cite: 1].

---

## 🚀 Execution Instructions (Run Order)

Our submitted code is designed to run from data loading to final results in a clear, executable order without depending on undocumented local paths[cite: 1].

**To reproduce our expected output:**
1. Open `notebook.ipynb` in Google Colab or your local Jupyter environment.
2. Verify that the `housing.csv` dataset is in the correct folder path.
3. Select **"Restart Kernel and Run All"**.
4. The notebook must be run from a clean kernel. It will sequentially execute our data audit, exploratory visualizations, leakage-safe preprocessing pipeline, and final model evaluations.

---

## ⚙️ Reproducibility Settings

*   **Random Seeds:** We have explicitly set a random state of `np.random.seed(42)` for our data splitting (`train_test_split`) and our stochastic models (Random Forest) to guarantee reproducible output.
