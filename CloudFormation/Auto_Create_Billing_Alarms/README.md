# Auto Create 3 Billing Alarms

This CF Template helps new users on AWS to automagically create 3 Billing Alerts with user input billing amounts to ensure you do not get any suprises at the end of the month.

This template creates 3 Billing Alarms in CloudWatch and 1 SNS notification.

1. Please ensure you execute this template only in the US East North Virginia Region as billing alarms for all regions are consolidated in this region.
2. The 3 thresholds are editable. Please input the values according to your budget.
3. Ensure you take immediate action once you get the 3rd alert because there will be no alerts after this and the total billing amount could theoretically run to infinity.
4. The Cloudwatch Alarms & SNS notifications that are created by this template ideally should not cost you anything as they fit very well within the Free Tier. If you are outside of the free tier, please review your total alarms count to ensure you are aware of how much additional this would cost you.
5. Please ensure you confirm the alert subscription that would come to your email address post creating this stack.
