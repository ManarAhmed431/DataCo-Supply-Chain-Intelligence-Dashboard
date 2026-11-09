# DataCo-Supply-Chain-Intelligence-Dashboard
An end-to-end analytics project built in Power BI that analyzes DataCo's supply chain orders (January 2015 – January 2018). It covers sales performance, profitability, delivery performance, and a machine learning model (Weka) that predicts late-delivery risk.

Project Overview

The report consists of four interactive pages:

Page	Focus
Executive Dashboard	High-level KPIs, monthly sales and profit trend, late delivery by shipping mode, profit by department, and regional performance
Shipping & Delivery	On-time vs. late performance, actual vs. scheduled delivery days, delivery status breakdown, late rate by market, and a shipping mode scorecard
Sales & Profitability	Net sales and margin by market, top categories by profit, customer segment mix, and departments ranked by loss-making item rate
Predictive Analytics	Late-delivery risk model: performance metrics, feature importance, confusion matrix, ROC curve, and predicted vs. actual late rate by shipping mode

Each page includes slicers (Year, Market, Department, Shipping Mode / Segment) for interactive filtering.

Key Metrics
Net Sales: $33M
Total Profit: $4M (12.0% margin)
Late Delivery Rate: 57.3% (cancelled shipments excluded)
Loss-Making Items: 18.7%
Average Order Value: $503
Average Discount: 10.1%
Key Insights
Late deliveries are systemic. Late rates are consistently 57–60% across all regions and markets, so the problem is not geographic.
Shipping mode drives lateness. First Class shows a 100% late rate and Second Class 79.8%, while Standard Class is only 39.8%. This points to unrealistic scheduled delivery promises for faster shipping tiers.
Fan Shop is the profit leader (~$1.83M), followed by Apparel and Golf.
Europe and LATAM generate the most revenue, with similar margins (~12%) across all markets.
Consumers account for about 52% of net sales.
Predictive Model
Tool: Weka
Validation: 10-fold cross-validation on 172,765 shipped order items
Results: Accuracy 71.5%, Precision 82.7%, Recall 63.6%, F1 71.9%, ROC AUC 0.771
Top features (information gain): Days Scheduled and Shipping Mode
Risk levels: High (≥ 70%), Medium (40–70%), Low (< 40%) predicted probability of late delivery
Tools & Technologies
Power BI Desktop (data modeling, DAX measures, interactive visuals)
Weka (classification and late-delivery risk prediction)
Notes
Late delivery % excludes cancelled shipments.
Delay Gap = Average Actual Days − Average Scheduled Days.
Profit is calculated per order item; loss-making means an item with negative profit.

