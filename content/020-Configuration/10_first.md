---
title: "Deploy the CloudFormation Stack"
chapter: false
weight: 10
---

## Deploy the CloudFormation Stack
Click here if you wish to deploy in [**us-east-1**](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://s3.us-east-1.amazonaws.com/aws-ml-blog-us-east-1/artifacts/lca/lca-main.yaml&stackName=LCA&param_installDemoAsteriskServer=true)

Click here if you wish to deploy in [**us-west-2**](https://us-west-2.console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/create/review?templateURL=https://s3.us-west-2.amazonaws.com/aws-ml-blog-us-west-2/artifacts/lca/lca-main.yaml&stackName=LCA&param_installDemoAsteriskServer=true)

### Input Your Parameters
![Stack Creation](/images/stackCreation.jpg)
Enter the following parameters and leave the ones not specified here blank:
- Stack Name: Choose any name for your stack

**Web UI Authentication** 
- Admin Email Address: The email address of the admin user to be used to log into the web UI. This should be your login email.
- Authorized Account Email Domain (Optional): Enter the email domain that is allowed to sign up and sign in using the WebUI. For example, you might limit it to just people who have your corporate email domain.

**Telephony Ingestion Options**
- Call Audio Source:  Choose Genesys Cloud Audiohook Web Socket

**Agent Assist Options**
- Enable Agent Assist: Choose QNABOT on AWS with the new Kendra Index (Developer Edition)

**Amazon S3 Configuration**
- Audio File Prefix: Leave this as is with the auto-populated option
- Call Analytics Output File Prefix: Leave this as is with the auto-populated option

**Amazon Transcribe Configuration**
- Enable Partial Transcripts: Set to true

    *This will enable partial transcripts _to receive _low-latency_ evolving transcriptions_ for each conversation turn.*
- Transcribe API mode: Set to 'Analytics'

    *This uses the Amazon Transcribe Real-time Call Analytics service, used to support call categories and alerts, call summarization, and PCA integration.*
- Enable Content Redaction for Transcripts: Set to true

    *This enables content redaction from Amazon Transcribe transcription*
- Language for transcription: Choose your appropriate language
- Content Redaction Type for Transcription: Choose PII
- Transcription PII Redaction Entity Types: Leave this as is with the auto-populated options

    *Allows you to select the PII entity types you want to identify or redact*
 
**Transcript Event Processing Configuration**
- Enable Sentiment Analysis: Set to true
- Lambda Hook Function Mode Non-Partial only: Set to true

    *Specifies if Transcript Lambda Hook Function (if specified) is invoked for Non-Partial transcript segments only (true)_, or both Partial and Non-Partial transcript segments (false).*

**Download Locations**
- Demo Asterisk Download URL: Leave as is

    *The URL used to download the Asterisk PBX software*
- Demo Asterisk Agent Audio URL: Leave as is

    *URL for audio (agent.wav) file download for demo Asterisk server*

**Amazon CloudFront Configuration**
- CloudFront Price Class: PriceClass_100

    *See the [CloudFront Pricing](https://aws.amazon.com/cloudfront/pricing/) for a description of each price class*

**Record Retention**
- Record Expiration in Days: Set to 90 for the workshop

    *The length of time, in days, that LCA will retain call records*

**User Experience**
- Category Alert Regular Expression: Set to '.*'

    *this regular expression will be used to show an alert in red in the web user interface if it matches a call category*

**Post Call Analytics (PCA) Integration**
- PCA InputBucket Transcript Prefix: Leave as is
- PCA InputBucket Playback AudioFile Prefix: Leave as is
- PCA Web App Call Path Prefix: Leave as is

## Run the Stack
After inputting all parameters, you are now ready to run the stack! Press create now. The creation of the stack takes approximately 30 minutes so go have a little break now. 