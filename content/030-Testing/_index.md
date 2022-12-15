---
title: "Testing"
chapter: true
weight: 30
---

## Logging into the AWS LCA and QNA Bot Consoles
Upon running the stack, the email you provided as the Admin Email Address would have received two emails with temporary passwords and links for logging into both the LCA Dashboard and the QNABot builder. The LCA Dashboard is where you can view live or historical calls that you place into your Genesys Cloud CX environment with real-time transcription, sentiment analysis and agent assist provided by AWS. The QNABot is where you can configure the backend of the agent assist features. We'll explore both of those dashboards in more detail in the sections following this one. First, we need to get you logged in!

Navigate to the email that you provided when you provided inputs for the CloudFormation stack. You should have received two emails from "no-reply@verificationemail.com". Those emails come with temporary passwords and links to the dashboards.
![LCAPassword](/images/LCAPassword.jpg)

For the LCA dashboard, simply provide your email and the temporary password provided. You will then be able to set a permanent password. 

For the QNABot dashboard, your username will be "Admin" and then you will use the temporary password provided. You will then be able to set a permanent password. 

To manage the users who have access to these dashboards, use Amazon Cognito. 