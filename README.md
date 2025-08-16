# PaySwift Feature Analysis

![](https://github.com/itsmearafik/PaySwift_Case_Study/blob/main/PaySwift_dashboard.png)

## Phase 1: Understanding the Data and Initial Thoughts
Before we even look at specific data (which you'll be providing), let's pre-emptively consider what we'll be looking for within each column you mentioned. This will help us formulate specific queries and analyses.
## Our Data Columns:
-	Userid: Unique identifier. Essential for grouping and understanding individual customer journeys.
-	Age: Demographic information. Could reveal age-related patterns in feature adoption, default risk, or churn.
-	Loan amount: The principal amount of the micro-loan. Crucial for understanding default rates in relation to loan size.
-	Repayment status [on-time, defaulted, late payment]: Our core metric for loan default analysis.
-	Feature used most [mobile, savings, loan service, budgeting, investment advice]: Key to understanding feature adoption and identifying underutilized services.
-	Month transactions: A proxy for engagement and activity level. Higher transactions might indicate higher engagement or vice-versa.
-	Churned [yes, no]: Our core metric for customer retention analysis.
-	Default risk [1-5]: An internal risk score. This is a powerful existing feature that we can leverage heavily. We need to understand how this score is assigned and its correlation with actual defaults.

## Initial Brainstorming - What to look for in each problem area:
1. Low adoption rates for new features:
* Questions:
* Which feature used most is most popular? Which are least popular?
* Is there a correlation between age and feature used most?
* Do month transactions differ significantly based on feature used most?
* Do users who churn (churned = 'yes') tend to use fewer features or specific features less?
* Potential Insights: Identify underperforming features and user segments not engaging with them.

2. High loan default rates:
* Questions:
* What is the overall distribution of repayment status?
* What is the average loan amount for defaulted vs. on-time payments?
* How does default risk correlate with actual repayment status? Is the internal risk model effective?
* Are there specific age groups with higher default rates?
* Do users who primarily use the loan service as their feature used most have higher default rates?
* Do month transactions (or lack thereof) before default indicate anything?
* Potential Insights: Identify high-risk segments, evaluate the effectiveness of the default risk score, and uncover contributing factors to defaults.

3. Customer churn:
* Questions:
* What's the overall churn rate?
* What feature used most do churned users tend to have? Did they only use one feature and then leave?
* How do month transactions for churned users compare to active users? Is there a decline in activity before churn?
* Are there specific age groups with higher churn rates?
* Is there a correlation between repayment status (especially late payment or default) and churned?
* Does a high default risk score correlate with churn, even if they haven't defaulted yet?
* Potential Insights: Identify churn drivers, early warning signs, and characteristics of customers at risk of churning.

## Phase 2: Data Analysis (Your Turn to Provide Data!)
Once you provide the actual data (even a sample or aggregated statistics if a full dataset isn't feasible right now), we'll move into the core analysis.

My Approach when you provide the data:
1.	Data Cleaning & Pre-processing (if necessary): Check for missing values, data types, and inconsistencies.
2.	Descriptive Statistics: Get a high-level overview of each column (means, medians, modes, distributions, counts).
3.	Univariate Analysis: Understand individual column distributions.
4.	Bivariate and Multivariate Analysis: This is where the real insights often emerge. We'll look at relationships between variables.
o	repayment status vs. loan amount, age, default risk, feature used most, month transactions.
o	churned vs. age, feature used most, month transactions, repayment status, default risk.
o	feature used most adoption rates vs. age, month transactions.
5.	Segmentation: We'll segment users based on key characteristics (e.g., age groups, default risk levels) to identify distinct patterns.

## Phase 3: Generating Business Insights & Recommendations
After the analysis, we'll synthesize our findings into concrete business insights and actionable recommendations, directly addressing the Head of Product's questions.
•	Increasing user engagement: Focus on popular features, cross-promotion, targeted onboarding for underused features.
•	Reducing default rates: Risk-based interventions, personalized repayment plans, early warning systems based on transaction patterns.
•	Improving customer retention: Identifying churn triggers, proactive engagement with at-risk customers, value proposition reinforcement.


“The features we build aren't just tools they are habits in disguise.”
Drive value, drive trust.

