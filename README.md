# AI-Driven-Sales-Forecasting-Marketing-Analysis-

**Sales Forecasting and Optimal Marketing Spend Allocation**

**Insight. Strategy. Impact.**
This project delivers a robust framework for **predicting future sales** and **optimally allocating marketing budgets** across different channels using a combination of **time-series forecasting (Prophet)** and **regression analysis**. It helps businesses make data-backed decisions to boost ROI and meet revenue goals.

---

### **Importance of Solving This Problem**

#### **Strategic Planning**

* **Inventory and Production Decisions:** Accurate sales forecasts inform how much stock to keep and when to produce, reducing both **overstocking and stockouts**.
* **Financial Forecasting:** Enables better budgeting and resource planning.

#### **Resource Optimization**

* **Marketing Budget Efficiency:** Understand which channels (TV, Radio, Newspaper) yield the best results, so money isn’t wasted on low-ROI campaigns.
* **Maximum Impact Per Dollar:** Make sure each marketing dollar directly contributes to **sales growth**.

#### **Competitive Advantage**

* **Trend Anticipation:** Businesses that forecast accurately can respond faster to market shifts.
* **Market Share Growth:** Outperform competitors by being proactive.

#### **Profitability Enhancement**

* **Cost Control:** Align operational decisions with expected revenue.
* **Revenue Maximization:** Drive growth through focused campaigns and smarter investments.

#### **Risk Mitigation**

* **Early Warning Signals:** Spot a downturn before it happens and take corrective actions.

---

### **Key Features**

#### **1. Data Loading & Preprocessing**

* Load `marketing_sales_data.csv`
* Convert `Date` to datetime and set as index
* Handle missing values
* Create time-based features (Month, Year)

#### **2. Exploratory Data Analysis (EDA)**

* **Sales Trends Visualization:** Spot seasonality and trends
* **Channel Spend Breakdown:** Understand how budget is currently distributed
* **Correlation Insights:** Determine which channels have the strongest initial influence on sales

#### **3. Sales Forecasting with Prophet**

* **Prophet Model:** Trained on historical sales data
* **Forecast Components:** Trend, seasonality (weekly, yearly)
* **Future Sales Prediction:** Visualized with confidence intervals

#### **4. Optimal Marketing Spend Allocation (Linear Regression)**

* **Regression Model:** Evaluates effect of each marketing channel on sales
* **Coefficient Analysis:** Quantifies **impact of TV, Radio, Newspaper**
* **Optimization Logic:** Allocates a fixed total budget to maximize predicted sales

#### **5. Model Evaluation**

* **Forecasting Metrics:** Visual comparison of actual vs. predicted
* **Regression Metrics:**

  * **Mean Squared Error (MSE)**
  * **R-squared (R2)** for model fit

---

### **Technology Stack**

* **Python** – Core development language
* **Pandas & NumPy** – Data wrangling and manipulation
* **Matplotlib & Seaborn** – Visual analytics
* **Prophet** – Time-series forecasting
* **Scikit-learn** – Regression modeling and evaluation
* **Jupyter Notebook** – Development environment

---

### **Getting Started**

#### **Prerequisites**

* Python 3.7+
* Jupyter Notebook or JupyterLab

#### **Installation Steps**

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install pandas numpy matplotlib seaborn prophet scikit-learn
```

#### **Run the Notebook**

```bash
jupyter notebook "Sales Forecasting and Optimal Marketing Spend.ipynb"
```

#### **Load the Dataset**

Ensure `marketing_sales_data.csv` is in the same directory as the notebook.

---

### **Usage Example – Budget Allocation**

```python
def allocate_marketing_budget(total_budget, linear_model):
    tv_spend = total_budget * 0.5
    radio_spend = total_budget * 0.3
    newspaper_spend = total_budget * 0.2

    print(f"Optimal Budget Allocation for a total of ${total_budget:,.2f}:")
    print(f"  TV: ${tv_spend:,.2f}")
    print(f"  Radio: ${radio_spend:,.2f}")
    print(f"  Newspaper: ${newspaper_spend:,.2f}")
```

---

### **Future Enhancements**

* **Advanced Time-Series Models:** ARIMA, SARIMAX, LSTMs
* **Dynamic Optimization:** Reinforcement learning or genetic algorithms
* **Interactive Dashboards:** Dash, Streamlit, Power BI for live inputs
* **Feature Expansion:** Add holidays, economic data, competitor activity
* **Scenario Planning:** Simulate spend and forecast impact interactively

---

### **Contact**

**Pranjal Patil** – \[(https://www.linkedin.com/in/pranjal-patil07/)]
Project Repository: \[(https://github.com/pranjalpatil-73/AI-Driven-Sales-Forecasting-Marketing-Analysis-)]
