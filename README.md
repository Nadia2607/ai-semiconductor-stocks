# ai-semiconductor-stocks
Semiconductor Market Analysis (Phase 1: Technology Research)
Overview
This project analyzes the global semiconductor market from 2012 to 2025, focusing on technology trends, profitability, and volatility. It leverages a dataset from Kaggle (Semiconductor Stocks and the AI Surge) and custom-collected event and company data. Phase 1 covers technology research, with Phase 2 (in development) planned for detailed player analysis. Visualizations are built in Power BI for interactive exploration.
Project Chronology
1. Initial Setup and Data Collection

Objective: Set up the environment and gather data.
Actions: Imported the Pandas library and verified the Kaggle dataset (semi_conductor_se.csv) availability using os.listdir(). The dataset covers 150 companies over 13 years.
Output: Initial DataFrame (df) created, with data integrity checked via df.isnull().sum().

2. Data Preparation

Objective: Clean and structure data for analysis.
Actions: Re-imported the dataset to resolve namespace issues and integrated supplementary data (e.g., event tags, company profiles). Prepared metrics like daily returns and volume ranks.
Output: Cleaned data ready for processing, aligned with Power BI requirements.

3. Exploratory Data Analysis (EDA)

Objective: Explore trends and key metrics.
Actions: Calculated daily returns and ranked companies by total volume. Identified patterns linked to market events (e.g., NVIDIA’s AI growth in 2024).
Output: Preliminary insights into top performers and volatility.

4. Clustering Analysis

Objective: Segment companies by volatility.
Actions: Applied K-Means clustering (4 clusters) on scaled daily return data, using StandardScaler for normalization.
Output: Cluster assignments generated, forming the basis for volatility-based visualizations.

5. Visualization Development with Power BI

Objective: Create interactive dashboards.
Actions: Imported cleaned data into Power BI to develop:
Dashboard 1 ("Market Snapshot"): Bar charts for 50 most profitable companies (e.g., NVIDIA at 6 трлн volume), 50 with average profitability (e.g., Formosa Sumco), and others with lowest profitability (e.g., Weebit Nano). A volatility chart shows daily return fluctuations, and a scatter plot links Avg Daily Return, Volatility, and MarketCapValue by Term of Outlook.
Dashboard 2 ("Analysis of the market by profitability leaders"): Bar chart for 50 companies with highest total volume (e.g., Micron Technology), a time-series volatility chart, and a bubble chart correlating Avg Daily Return, Volatility, and Term of Outlook.
Filters: Activity Sphere (e.g., Semiconductor, Materials) and Tech Subcategory (e.g., AI Chips) for niche exploration.


Output: Interactive dashboards accessible in Power BI, with static snapshots available for reference.

6. Documentation and Refinement

Objective: Document the process for GitHub.
Actions: Added comments to the Jupyter Notebook and prepared this README. Ensured data compatibility with Power BI measures and tables.
Output: Project ready for sharing, with users able to interact with visualizations.

Technology Stack

Programming Language: Python
Libraries: Pandas, NumPy, Scikit-learn
Tools: Jupyter Notebook, Power BI, GitHub
Data Source: Kaggle - Semiconductor Stocks and the AI Surge

Installation and Usage

Clone the Repository:
git clone https://github.com/Nadia2607/ai-semiconductor-stocks.git 
cd ai-semiconductor-stocks


Install Dependencies:
pip install -r requirements.txt

(Create requirements.txt with pandas, numpy, scikit-learn.)

Run the Analysis:

Open the Jupyter Notebook (Ai%20semiconductor%20(2).ipynb) to replicate the code.
Import data into Power BI (ai-semiconductor.pbix) for interactive dashboards.



Visualizations Explained

50 Most Profitable Companies: Bar chart showing volume leaders (e.g., NVIDIA at 6 трлн), indicating market dominance.
Volatility Chart: Line graph of daily return ranges (Min, Max, Avg) for companies like AMD and TSMC, reflecting risk levels.
Avg Daily Return vs. Volatility: Scatter plot with bubbles sized by MarketCapValue, color-coded by Term of Outlook (Cautious, Long-term, Strong), showing growth-risk dynamics.
Volume Leaders: Bar chart of top 50 by total volume, highlighting key players.
Filters: Use Activity Sphere and Tech Subcategory to drill into niches (e.g., AI Chips, Materials).

Insert Jupyter Notebook and Power BI Document

Jupyter Notebook: [Ai semiconductor (2).ipynb](Ai%20semiconductor%20(2).ipynb) 
Power BI Document:[ai-semiconductor.pbix](ai-semiconductor.pbix)

Future Work (Phase 2)

Detailed analysis of top companies.
Enhanced visualizations with additional tools.
Real-time data integration.

Contributing
Fork this repository, submit issues, or suggest improvements to code or visualizations.
License
MIT License - See the LICENSE file for details.
Acknowledgments

Thanks to Kaggle for the dataset and the xAI community for support.

