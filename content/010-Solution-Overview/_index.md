---
title: "Solution Overview"
chapter: true
weight: 10
---

# Solution Overview
This Workshop contains instructions to showcase a sample service that implements the Genesys Audiohook protocol and leverages a variety of AWS services. The implementation includes the following:
1.	ingestion of audio stream from Genesys Cloud via Audiohook protocol
2. transcription of the audio stream to text using Amazon Transcribe streaming SDK
3.	integration of transcriptions into the Live Call Analytics with Agent Assist (LCA) sample solution

![Architecture](/images/architecture.png)

**IMPORTANT**

The code used in this workshop is provided as a sample blueprint to get started building an Audiohook server and test protocol compliance. It does not include some of the robustness and resiliency patterns that you will likely require for a production-quality service.
