# Practical Application III: Comparing Classifiers

This project focuses on building and evaluating machine learning models to predict whether a client will subscribe to a term deposit. The dataset comes from the UCI Machine Learning Repository and includes data on client demographics and campaign interactions.

**Objective**: To determine the best-performing classifier and provide actionable recommendations for improving marketing strategies.
## Dataset Description

The dataset contains information on clients of a Portuguese bank and their interaction with marketing campaigns. Key features include:

- **Demographics**: Age, job, marital status, education.
- **Campaign interactions**: Contact method, previous outcomes, number of contacts.
- **Economic indicators**: Employment variation rate, consumer confidence index.
- **Target Variable**: `y` (whether the client subscribed to a term deposit).
## Project Workflow

1. **Data Preprocessing**:
   - Handled missing values and addressed class imbalance using SMOTE.
   - Encoded categorical features and transformed skewed numeric features.

2. **Model Building**:
   - Implemented and tuned Logistic Regression, k-Nearest Neighbors, Decision Tree, and Support Vector Machine.

3. **Evaluation**:
   - Evaluated models using metrics like accuracy, precision, recall, and F1-score.
   - Compared models using visualizations and consolidated results.

4. **Findings and Recommendations**:
   - Identified the best-performing model (SVM) and provided actionable insights for marketing optimization.
## Findings and Recommendations

### Best Model
The Support Vector Machine (SVM) emerged as the best-performing model:
- **Accuracy**: 86.53%
- **Precision (Class 0)**: 91%
- **Recall (Class 0)**: 94%
- **F1-Score (Class 0)**: 93%

1. **Target high-potential clients**: Focus marketing efforts on middle-aged clients in administrative jobs, who are most likely to subscribe.
2. **Refine Class 1 predictions**: Address the challenges of minority class prediction by adjusting the decision threshold or using advanced resampling techniques.
3. **Continuous Model Improvement**: Retrain the model periodically with updated data to maintain performance.

## Recommendations for the Bank’s Marketing Strategy:
Summary of Insights:
1.	Demographics Matter:
- Clients aged 35–50, particularly those in administrative jobs, exhibit a higher likelihood of subscribing to term deposits.
- Clients with prior successful subscriptions are more receptive to new offers.
  
2.	Campaign Features Impact Success:
-	The success of previous campaigns (e.g., campaign duration, number of contacts) directly correlates with the likelihood of client subscription.
-	Features like contact duration, when included, significantly improve model predictions, although this is not actionable before contact.

### Actionable Recommendations:

1. Segment and Prioritize High-Potential Clients:
•	Focus marketing resources on middle-aged professionals, particularly in administrative and managerial roles, as they are more likely to subscribe.
•	Use customer segmentation tools to refine lists for targeted outreach.

How:

•	Tailor campaigns specifically for this group with messaging around stability, financial growth, and the security of term deposits.
•	Highlight benefits like competitive interest rates or flexible terms in campaign messages.

2. Leverage Data from Previous Campaigns:
-	Prioritize clients who previously interacted with the bank (e.g., engaged but did not subscribe or already subscribed to other products).
•	Focus on re-engaging clients who participated in past campaigns with personalized offers or follow-ups.

How:

•	Utilize predictive analytics to rank clients by likelihood to subscribe.
•	Send follow-up emails or make phone calls targeting this segment with reminders of past campaign offers.

3. Enhance Campaign Strategies:
    
•	Reduce redundant contacts with low-potential groups (e.g., students or retired clients), saving resources for high-yield demographics.
•	Experiment with shorter, high-quality contacts instead of prolonged engagement, based on campaign performance data.

How:

•	Shorten the duration of calls for non-responsive groups and reallocate efforts to groups with higher engagement rates.

5. Optimize Communication Channels:
   
•	Focus on email campaigns and phone calls as primary communication methods. These are shown to perform better in engaging clients.
•	Test alternative channels (e.g., social media ads targeting mid-career professionals) to expand outreach.

How:

•	Invest in tools to track client responses across different channels and analyze which method yields the best results.

6. Address Class Imbalances in Data:
   
•	Implement strategies like undersampling low-yield client groups or SMOTE techniques to balance data for future modeling.How:

•	Use insights from models to understand and counter biases in datasets, ensuring future campaigns don't exclude overlooked potential clients.

7. Monitor and Refine Campaigns:
   
•	Continuously track campaign performance metrics such as subscription rates, response times, and churn rates.

•	Adapt strategies based on model predictions and ongoing campaign outcomes.

How:

•	Conduct quarterly reviews of campaign success rates and compare them to predictions made by the machine learning models. Use these insights to recalibrate client segmentation and targeting.
Visualization Support: Include charts such as:

•	Bar Graphs: Subscription rates by job type, age group, or education level.

•	Pie Charts: Distribution of clients who subscribed vs. did not.

•	Heatmaps: Correlation between key features and subscription likelihood.

For more details with the full analysis and visualization visit ComparingClassifiers.ipynb Jupiter Notebook

## Acknowledgments

- Dataset from the UCI Machine Learning Repository.


Anlysis by Nohelia Gil.
