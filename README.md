# Project_Profit_Analyst
This project focuses on analyzing company profit and loss data.  I used Excel and SQL to clean, filter, and organize the data.  Profit trends were analyzed by product, region, and time period.  The analysis helped identify high-profit and low-profit areas.  Insights from this project support better business decision-making.



PRDA-01 Profit Analysis Report
Assessing the Impact of Operational Spending on Startup Profitability
Debendra Malik
debendramalik267@gmail.com | 8144767737
Project Duration: 28/11/2025 to 30/11/2025
1 Executive Summary and Project Goal
The primary objective of the PRDA-01 project was to apply Multiple Linear Regression to a dataset of 50 startups to quantify the relationship between key operational expenses (R&D, Administration, and Marketing Spend) and final Profit.
The analysis confirms that R&D Spending is the single most significant driver of Profit, exhibiting a high positive correlation. Conversely, Administration Spending shows a negligible or slightly negative impact. Recommendations focus on strategically reallocating resources to maximize investment in research and development.
2 Data Acquisition and Exploratory Analysis (EDA)
The dataset comprises 50 startup records across three states: New York, California, and Florida.
2.1 Feature Attributes
•
R&D Spending: Investment in research and development.
•
Administration Spending: General operational and overhead costs.
•
Marketing Spending: Expenditure on marketing and advertising.
•
State: Location of the startup.
•
Profit: The dependent (target) variable.
2.2 Key Findings from EDA • Correlation: R&D Spending showed the strongest linear relationship with Profit (0.97), indicating that almost all variation in profit is explained by R&D investment. Marketing Spending also showed a strong positive correlation (0.75).
• State Impact: Average profit across the three states (NY, CA, FL) showed minimal variance, suggesting that spending ratios are far more influential than geographic location.
3 Multiple Linear Regression Model
A Multiple Linear Regression model was constructed to isolate and measure the contribution of each spending category to the total profit. Image of multiple linear regression model diagram
3.1 Model Formulation
The model estimates the profit (Y ) as a linear combination of the independent spending variables
Profit/Y = b0 + b1*(R&D Spend) + b2*(Administration) + b3*(Marketing Spend)
Where (b0) are the regression coefficients and Standard the error term.
3.2 Coefficient Analysis
The table below summarizes the theoretical coefficients, representing the change in Profit for every unit change in the corresponding spending, holding other factors constant. Table 1: Regression Coefficient Analysis (Simulated Data)
SUMMARY OUTPUT
Regression Statistics
Multiple R
0.975062
R Square
0.950746
Adjusted R Square
0.947534
Standard Error
9232.335
Observations
50
ANOVA
df
SS
MS
F
Significance F
Regression
3
75683964196
2.52E+10
295.9781
4.53E-30
Residual
46
3920856301
85236007
Total
49
79604820497
Spending Category
Coefficients
Standard Error
t Stat
P-value
Lower 95%
Upper 95%
Lower 95.0%
Upper 95.0%
Intercept
50122.19
6572.353
7.626218
1.06E-09
36892.73
63351.65
36892.73
63351.65
RD_Spend
0.805715
0.045147
17.84637
2.63E-22
0.714838
0.896592
0.714838
0.896592
Administration
-0.02682
0.051029
-0.52551
0.601755
-0.12953
0.0759
-0.12953
0.0759
Marketing_Spend
0.027228
0.016451
1.655077
0.104717
-0.00589
0.060343
-0.00589
0.060343
4 Profit Prediction and Recommendations
4.1 Profit Prediction Results
The trained model was used to predict profit for the two specified input scenarios: Table 2: Predicted Profit for Given Scenarios
R&D spend
Administration
Marketing_spend
profit
21892.92
81910.77
164270.7
70037.9
23940.93
96489.63
137001.1
70554.57
4.2 Strategic Recommendations
Based on the high R2 value (high model fit) and the quantified coefficients, the following strategic recommendations are proposed:
1.
Maximize R&D Investment: Since every dollar spent on R&D Returns = 0.805715 in profit, R&D should be treated as the primary growth engine. Reallocate funds from less impactful areas to this category.
2.
Optimize Administrative Efficiency: The negative or negligible coefficient for Administration suggests that this spending category does not contribute to profit. Focus efforts on process automation and lean management to reduce administrative overheads without impacting core operations.
3.
Strategic Marketing Support: Marketing is a positive contributor but is far less impactful than R&D. Utilize marketing funds strategically to support the launch and scaling of R&D-developed products, rather than as an independent growth driver.
5 Visualization Summary (PowerBI/Tableau)
The visualization is critical for communicating the findings to stakeholders
