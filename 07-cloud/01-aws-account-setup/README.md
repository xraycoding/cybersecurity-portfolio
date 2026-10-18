\# AWS Account Setup: Secure It Before Building On It



\## Goal

Lock down a brand new AWS account before building anything, so a mistake or a stolen password can't turn into a big bill or a full account takeover.



\## What I did



1\. \[Billing alarm](01-billing-alarm/): set up cost alerts so I hear about unexpected spending early.

2\. \[Root user MFA and lockdown](02-root-mfa/): protected the all-powerful root user.

3\. \[Non-root admin user](03-admin-user/): moved daily work to a limited identity.



\## Why this order

Cost protection first so early mistakes can't get expensive. Then the root user, which has unrestricted control, gets locked down. Then I stop using it and work as a normal admin user.



\## What's next

CloudTrail, GuardDuty and Security Hub, then scanning the account with Prowler.

