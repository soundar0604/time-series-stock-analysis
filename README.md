### requirements.txt
pandas
numpy
matplotlib
statsmodels
scikit-learn


### README.md
# 📈 Stock Price Time Series Analysis

This project analyzes stock price data for different companies using ARIMA models.  
It generates plots showing stock prices over time and forecasts future trends.

---

## 🚀 Features
- Load stock price data from **CSV** (`Q3_Q4_stock_data.csv`).
- Preprocess data (handle missing values, date parsing).
- Train an **ARIMA model** for each company.
- Generate plots:
  - Stock price over time.
  - Train vs Test vs Forecast.
- Save plots into the `plots/` directory.
- Evaluation metrics: **MSE** and **RMSE**.

---

## 📂 Project Structure

.
├── Time_Series_Analysis.py   # Main script
├── Q3_Q4_stock_data.csv      # Input dataset
├── requirements.txt          # Python dependencies
├── plots/                    # Generated plots (ignored in repo)
└── .github/workflows/        # GitHub Actions workflows




## ⚙️ Installation

Clone the repo and install dependencies:

bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
pip install -r requirements.txt




## ▶️ Usage

Run the analysis script:

BASH
python Time_Series_Analysis.py

---

Plots will be saved in the 'plots/' directory.

---

## 🤖 GitHub Actions Workflow

This project includes a CI workflow that:
- Installs dependencies.
- Runs 'Time_Series_Analysis.py'.
- Uploads generated plots as **artifacts** in the Actions tab.

You can manually trigger the workflow or it runs automatically on pushes.

📊 Example Output

{Company}_stock_price_plot.png` saved inside `plots/`.
- Example evaluation metrics printed to console:
- Company A - MSE: 123.45, RMSE: 11.11
