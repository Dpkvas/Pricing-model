# Natural Gas Pricing Model 💰🔥

This project simulates a simplified pricing model for natural gas, inspired by real-world trading desk requirements. The project is implemented in Python using Jupyter Notebooks and is designed to estimate future gas prices and price storage contracts based on configurable parameters.

---

## 📁 Project Structure

- `data/Nat_Gas.csv`: Historical monthly natural gas prices from October 2020 to September 2024.
- `notebooks/jp_morgan.ipynb`: 
  - Cleans and analyzes the natural gas price data.
  - Builds a price estimator to return the price on any input date.
  - Forecasts prices one year into the future.
  - Explores seasonal trends and visual patterns.
- `notebooks/pricing_model.ipynb`:
  - Implements a function to price a gas storage contract.
  - Takes into account injection/withdrawal dates, rates, volume limits, and storage costs.
  - Returns a contract valuation for client use.
- `notebooks/task_3_credit_risk.ipynb`:
  - Trains models to estimate the Probability of Default (PD) for borrowers.
  - Calculates Expected Loss (EL) assuming a 10% recovery rate.
  - Compares multiple classification models and their performance.
  - Produces a function that returns EL for given borrower details.
---

## 📌 Key Features

### ✅ Task 1: Price Estimation

- Reads historical monthly natural gas prices.
- Implements a date-based price estimator using interpolation or time series modeling.
- Forecasts future prices using extrapolation.
- Visualizes seasonal and temporal trends in gas pricing.

📌 *Notebook*: `jp_morgan.ipynb`

### ✅ Task 2: Storage Contract Valuation

- Generalized function for pricing storage contracts.
- Supports flexible inputs:
  - Injection & withdrawal dates
  - Commodity buy/sell prices
  - Injection/withdrawal rates
  - Maximum storage capacity
  - Per-unit storage cost
- Outputs the net value of the contract.

📌 *Notebook*: `pricing_model.ipynb`

---
### ✅ Task 3: Credit Risk Analysis

- Loads borrower data including income, outstanding loans, and default history.
- Trains classification models to estimate the **Probability of Default (PD)**.
- Calculates **Expected Loss (EL)** on a loan assuming a 10% recovery rate.
- Supports different modeling techniques (Logistic Regression, Decision Tree, etc.).
- Provides a comparative performance summary of all tested models.
- Outputs a function that returns the expected loss given borrower features.

📌 *Notebook*: `task_3_credit_risk.ipynb`
---

## 📈 Sample Output

![Price Forecast Plot](images/sample_forecast.png) <!-- Optional: add if you include output visuals -->

---

## 🛠️ Technologies Used

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📦 Getting Started

```bash
git clone https://github.com/Dpkvas/Pricing-model.git
cd Pricing-model
pip install -r requirements.txt
