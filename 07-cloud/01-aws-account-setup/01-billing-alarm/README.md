\# Billing Alerts: Get Warned Before the Bill Arrives



\## Goal

Get alerted before a learning account generates unexpected costs. Cloud mistakes are easy to make and billing alerts are the safety net.



\## Part 1: Turned on AWS Free Tier alerts



I enabled Free Tier alerts in Billing preferences, delivered to the root user's email address. These warn me when my usage is approaching or exceeding the Free Tier limits.



\## Part 2: Created a monthly budget



I created a monthly cost budget of $10 in AWS Budgets, with 80% alert threshold that notifies me by email as spending approaches the limit.



!\[Budgets list showing My Monthly Cost Budget at $10.00 with thresholds OK and health status Healthy](../assets/billing-budget-created.png)



The budget shows a $10.00 limit, its thresholds are OK, and its health status is Healthy, so it is active and spending is currently under the limit.



\## Why I didn't build a CloudWatch billing alarm



A CloudWatch billing alarm is another way to do this, but it needs extra services (CloudWatch and SNS) and I wasn't sure of the cost. Budgets plus Free Tier alerts already cover what I need, so I kept the setup simple.



\## What I learned

\- Budgets and Free Tier alerts are different: a budget tracks spending against a limit, Free Tier alerts track usage against free allowances.

\- Alerts are notifications, not hard caps. They tell me, they don't stop spending.

\- Checking pricing before enabling a service is part of using the cloud safely.



\## Next steps

\- Consider adding a CloudWatch billing alarm once I've confirmed it stays within the Free Tier.

