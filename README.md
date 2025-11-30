# 📦 Supply Chain KPI Dashboard

> **Description:** A Python and Plotly-based dashboard analyzing key supply chain KPIs, including inventory optimization, stockout risk, and logistics performance.

## 🎯 Project Goal

The primary objective of this project is to simulate and analyze the performance of a logistics and inventory operation over a one-year period. By generating realistic time-series data and calculating essential Key Performance Indicators (KPIs), we aim to:

1.  **Identify Bottlenecks:** Pinpoint specific product categories or routes suffering from high **stockout risk** or **low delivery reliability**.
2.  **Drive Actionable Insights:** Programmatically generate recommendations (e.g., increase safety stock, review carrier performance) based on the calculated metrics.
3.  **Visualize Performance:** Create an interactive, shareable dashboard using **Plotly** to provide an at-a-glance view of the supply chain health.

## 🛠️ Technology and Tools

| Tool | Purpose | Why We Used It |
| :--- | :--- | :--- |
| **Python** | Core data generation and analytical engine. | Versatility and robust data science ecosystem. |
| **Jupyter Notebook** | Environment for reproducible, step-by-step analysis. | Excellent for data storytelling and showcasing code, output, and visualizations sequentially. |
| **Pandas & NumPy** | Data manipulation, aggregation, and synthetic data creation. | Standard industry tools for handling structured data efficiently. |
| **Plotly Express** | Interactive dashboard visualizations. | Generates dynamic, web-ready charts that look professional in a portfolio and allow users to hover for details. |

## 📊 Key Performance Indicators (KPIs)

The analysis focuses on measuring three critical areas of supply chain efficiency:

1.  **Stockout Frequency:** Total days a product's demand exceeded its available inventory.
2.  **On-Time Delivery Rate:** Percentage of shipments delivered successfully within the committed lead time.
3.  **Lead Time Distribution:** Analysis of the variability and consistency of the time required to receive stock.

## ⚙️ How the Analysis Works (Code Breakdown)

The Jupyter Notebook is structured into the following analytical phases:

### **Phase 1: Data Simulation**
* **What we did:** Generated **synthetic data** for 365 days across product categories.
* **Why we did it:** This demonstrates the ability to structure and model realistic **supply chain data** containing dimensions like inventory, demand, lead times, and delivery status, independent of external datasets.

### **Phase 2: Metric Calculation**
* **What we did:** Created new columns to flag **stockout days** and calculated the **Inventory Turnover Ratio** (Demand / Inventory).
* **Why we did it:** These calculated metrics form the foundation of our KPIs and allow us to move from raw data to actionable business performance indicators.

### **Phase 3: Visualization Dashboard**
* **What we did:** Used **Plotly Subplots** to combine four key charts (Demand by Product, Inventory vs. Demand, On-Time Rate, and Lead Time Histogram) into a single, cohesive dashboard layout.
* **Why we did it:** This provides a quick visual diagnosis of performance across the entire supply chain.

### **Phase 4: Automated Insights**
* **What we did:** Programmatically identified the worst-performing product for **stockouts** and the worst product for **delivery reliability**. We also used **Pandas Styler** to create a color-coded, heat-map summary table.
* **Why we did it:** This is the most crucial step—it shows the ability to translate technical output into **direct, actionable business recommendations**, moving beyond reporting into decision support.

## 🚀 Getting Started

To run this project locally, clone the repository and install the dependencies:

```bash
# Clone the repository
git clone [https://github.com/YourUsername/supply-chain-analytics-dashboard.git](https://github.com/YourUsername/supply-chain-analytics-dashboard.git)
cd supply-chain-analytics-dashboard

# Create a virtual environment (Recommended)
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

# Install required libraries from requirements.txt
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook Project_Notebook.ipynb
