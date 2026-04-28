Bank-Marketing-Prediction
Predicting Bank Marketing Campaign Success
This project uses machine learning to predict whether a customer will subscribe to a bank term deposit, helping marketing teams target the right people more effectively.

The Business Problem
Banks spend significant time and money on marketing campaigns, but many customer contacts do not lead to successful subscriptions. Predicting which customers are more likely to respond can reduce wasted outreach, improve campaign efficiency, and increase conversions.

The Data
This project uses a bank marketing dataset containing customer demographic information, past campaign details, and economic indicators. The dataset includes variables such as age, job type, education, number of contacts, month of contact, previous campaign outcome, and interest-rate-related indicators.

Key Discoveries
Clients in professional and retired occupations show noticeably higher subscription rates than other job groups: Younger clients and students also show moderate engagement, while manual and administrative jobs have lower response rates. This suggests the campaign may perform better when targeting financially stable or older customer segments, who may be more interested in savings products like term deposits.
Call duration appears strongly related to campaign success.: Clients who eventually subscribed typically had longer phone conversations with bank representatives, suggesting that engagement during the call plays an important role in conversion. Additionally, customers contacted repeatedly during the campaign show declining success rates, indicating that aggressive repeated calls may reduce effectiveness.
Subscription rates vary noticeably across months: Campaigns conducted in March, September, and October show higher success rates, while summer months show lower engagement. This pattern may reflect broader economic or seasonal financial behavior, suggesting the bank could prioritize marketing efforts during higher-performing months to improve campaign efficiency.
Visualizing the Story
Customers in professional and retired roles show higher subscription rates, suggesting targeted outreach can significantly improve conversion efficiency.(Subscription Rate by job.png)

Prediction Model
A Gaussian Naive Bayes model was developed to predict whether a client will subscribe. The model achieves strong overall accuracy, correctly identifying most non-subscribers while capturing a portion of high-value customers.

However, the confusion matrix reveals an important trade-off: the model misses some potential subscribers (false negatives), which represent lost revenue opportunities. From a business perspective, improving recall (capturing more “yes” clients) is more valuable than minimizing extra calls.

Recommendations
Action: Prioritize longer, high-quality client conversations Data shows that longer calls significantly increase subscription likelihood. Training agents to improve engagement could increase conversion rates by 10–15%, translating into hundreds of additional accounts per campaign..
Action: Target high-probability customer segments first Professionals, retirees, and previously successful contacts show higher conversion rates. Focusing outreach on these groups can reduce wasted calls and increase ROI..
Action: Limit repeated contact attempts Conversion rates drop with multiple calls. Reducing excessive follow-ups can lower operational costs while maintaining effectiveness.
Action: Use predictive scoring to guide outreach strategy Instead of mass calling, the bank should prioritize the top 30–40% of predicted high-probability clients. This can reduce outreach volume while maintaining — or even increasing — total conversions.
Tools & Techniques
Python | Pandas | Scikit-Learn | Matplotlib | Seaborn | Gaussian Naive Bayes | Google Colab

This project was completed as part of ISOM 835: Predictive Analytics at Suffolk University's Sawyer Business School. '''

print(readme_template)
