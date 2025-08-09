Cubic Zirconia Price Prediction (EDA & Regression)
Overview:
This project focuses on Exploratory Data Analysis (EDA) and Regression Modeling using the cubic_zirconia.csv dataset. The dataset contains various features of cubic zirconia stones (such as dimensions, weight, and cut) and their corresponding prices.
The main goal is to analyze factors affecting price and build a model to predict the price based on these features.

Dataset Information:
Dataset: cubic_zirconia.csv
Number of Rows: [insert after check]
Number of Columns: [insert after check]

Columns:
carat – Weight of the stone
cut – Quality of the cut (e.g., Ideal, Premium, Good)
color – Stone color rating (D best → J worst)
clarity – Measure of how clear the stone is
depth – Total depth percentage
table – Width of the top of the stone relative to widest point
x, y, z – Dimensions in mm
price – Price of the stone (Target variable)

🛠 Project Workflow:

1️⃣ Data Loading & Inspection
Loaded dataset using Pandas
Checked for missing values & data types
Performed descriptive statistics

2️⃣ Data Cleaning
Handled missing values
Removed duplicates
Corrected inconsistent values in cut, color, and clarity columns

3️⃣ Exploratory Data Analysis (EDA)
Univariate Analysis – Distribution of price, carat, and other features
Bivariate Analysis – Relationship between carat & price, cut & price
Multivariate Analysis – Combined impact of multiple features on price
Correlation Heatmap – To find strongest predictors for price

4️⃣ Feature Engineering
Converted categorical variables (cut, color, clarity) into numeric using Label Encoding / One-Hot Encoding
Created new feature: volume (x * y * z)

5️⃣ Model Building
Split data into train/test sets
Applied Linear Regression and Random Forest Regressor
Tuned hyperparameters for better accuracy

6️⃣ Model Evaluation
Metrics used: R² score, Mean Absolute Error (MAE), Root Mean Squared Error (RMSE)
Compared performance of different models

📊 Results & Insights
Carat was the most significant factor affecting price
Cut quality and clarity also had a notable effect, but less than carat
Random Forest outperformed Linear Regression with higher R² and lower error values

📈 Visualization Examples
Price vs Carat scatter plot
Boxplots of price distribution by cut and clarity
Correlation heatmap for all features

🖥️ Technologies Used
Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)

Jupyter Notebook for analysis and visualization

🚀 How to Run the Project
Clone this repository:

bash
Copy
Edit
git clone <your-repo-link>
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Open the Jupyter Notebook:

bash
Copy
Edit
jupyter notebook cubic_zirconia_EDA.ipynb

📌 Future Improvements
Try XGBoost and Gradient Boosting for better predictions

Deploy model as a Flask/Django API

Integrate a price recommendation web app
