Project Title: Digital Marketing Performance Analysis: Facebook vs. AdWords (A/B Testing)

Analyzing historical campaign data to compare Facebook and AdWords effectiveness and provide strategic advice for budget allocation and optimization to increase ROI.

Table of Contents

<a href="#overview">Overview</a>

<a href="#business-problem">Business Problem</a>

<a href="#research-questions-key-findings">Research Questions & Key Findings</a>

<a href="#dataset-assumptions">Dataset & Assumptions</a>

<a href="#tools-technologies">Tools & Technologies</a>

<a href="#project-structure">Project Structure</a>

<a href="#data-cleaning-preparation">Data Cleaning & Preparation</a>

<a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA) & Key Insights</a>

<a href="#final-recommendations">Final Recommendations</a>

<a href="#future-work">Future Work</a>

<a href="#how-to-run-this-project">How to Run this Project?</a>

<a href="#author-contact">Author & Contact</a>

<h2 id="overview">Overview</h2>

This project focuses on a comparative analysis (A/B Test) of two concurrent digital advertising campaigns: one run on Facebook and the other on AdWords. The primary goal is to determine the optimal platform for maximizing return on investment (ROI) by evaluating performance metrics such as clicks, conversions, and cost-effectiveness.

The findings from this analysis provide actionable recommendations for strategic budget reallocation and campaign optimization to deliver superior results for marketing clients.

<h2 id="business-problem">Business Problem</h2>

As a marketing agency, our primary objective is to maximize the return on investment (ROI) for our clients' advertising campaigns. We have conducted two ad campaigns, one on Facebook and the other on AdWords, and we need to determine which platform yields better results in terms of clicks, conversions, and overall cost-effectiveness. By identifying the most effective platform, we can allocate our resources more efficiently and optimize our advertising strategies to deliver better outcomes for our clients.

<h2 id="research-questions-key-findings">Research Questions & Key Findings</h2>

Research Question

Key Finding

Which ad platform is more effective?

Facebook demonstrated superior performance. Clicks on Facebook Ads show a strong positive correlation ($\mathbf{0.87}$) with conversions, compared to AdWords' moderate positive correlation ($\mathbf{0.45}$).

How does conversion performance differ?

Facebook consistently had more frequent days with higher conversions (categories $\mathbf{10+}$) than AdWords, which primarily clustered in the "less than 6" category.

Are there long-term stability in performance?

Cointegration Test: A long-term equilibrium relationship between Facebook advertising spend and conversions was confirmed.

What are the optimal times for Facebook advertising?

Conversions are highest on Mondays and Tuesdays.

When is the Cost Per Conversion (CPC) lowest?

May and November recorded the lowest Cost Per Conversion values, making them the most cost-effective months.

<h2 id="dataset-assumptions">Dataset & Assumptions</h2>

Dataset: marketing_campaign.csv

The dataset covers 365 days of campaign data throughout the year 2019, with one row for each day, including performance metrics for both Facebook and AdWords campaigns.

Key Features:

Date

Ad Views, Ad Clicks, Ad Conversions

Cost per Ad

Click-Through Rate (CTR), Conversion Rate, Cost per Click (CPC)

Assumptions:

The data accurately reflects all marketing costs and campaign performance for the year 2019.

The conversion metric is the primary indicator of business success.

<h2 id="tools-technologies">Tools & Technologies</h2>

This project was developed using a standard Python data science stack:

Programming: Python 3.x

Libraries: pandas, NumPy, matplotlib, seaborn, SciPy, Scikit-learn, statsmodels.

<h2 id="project-structure">Project Structure</h2>

This project is primarily a data analysis workflow documented in a single script or notebook.

.
├── marketing_campaign.csv  # Raw data file
└── facebook_ads_vs_google_ads-A-B_Testing-Python.ipynb    # Main notebook
└── README.md


<h2 id="data-cleaning-preparation">Data Cleaning & Preparation</h2>

This phase involved:

Date Conversion: Converted the Date column to datetime objects.

Numeric Cleaning: Removed $ and % symbols from monetary and rate columns and converted them to floating-point numbers.

Feature Engineering: Created categorical conversion columns (Facebook Conversion Category, AdWords Conversion Category) for comparative analysis.

<h2 id="exploratory-data-analysis-eda">Exploratory Data Analysis (EDA) & Key Insights</h2>

EDA focused on visualizing and statistically comparing performance:

Distribution: Clicks and conversions showed generally symmetrical distributions with few extreme outliers.

Conversion Comparison: Facebook significantly outperformed AdWords in generating high-conversion days.

Correlation: Confirmed the strong positive linear relationship between Facebook clicks and conversions ($\mathbf{0.87}$) compared to the moderate relationship for AdWords ($\mathbf{0.45}$).

Time Series: Identified Mondays and Tuesdays as peak conversion days and May/November as months with the lowest Cost Per Conversion.

<h2 id="final-recommendations">Final Recommendations</h2>

Prioritize Facebook Allocation: Allocate the majority of the budget to Facebook given the superior conversion correlation ($\mathbf{0.87}$).

Optimize Budget Timing: Increase budget focus on Mondays and Tuesdays for weekly pushes, and strategically allocate more budget to May and November due to lower Cost Per Conversion.

Investigate AdWords: Conduct further diagnostic research to identify specific factors influencing the moderate performance of the AdWords campaigns for optimization.

<h2 id="future-work">Future Work</h2>

Forecasting: Implement time series models to forecast future conversion rates and costs.

<h2 id="how-to-run-this-project">How to Run this Project?</h2>

Clone the Repository: (Assuming the code is in a repository).

Install Dependencies:

pip install pandas matplotlib seaborn numpy scikit-learn statsmodels


Run the Analysis: Execute the analysis script/notebook.

python analysis_script.py


<h2 id="author-contact">Author & Contact</h2>

Author: Shazmeen Shaikh
Contact: https://www.linkedin.com/in/shazmeen-shaikh-30bb63237/