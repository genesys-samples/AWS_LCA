---
title: "Configuration"
chapter: true
weight: 20
---

## Configuration
The configuration of this integration is broken up into two parts. 

1. Deploy the CloudFormation Stack in AWS - In this section, we will walk you through deploying a CloudFormation Stack in AWS. The CloudFormation will deploy 3 main components: 
    - QNABOT - QnABot conveniently orchestrates Amazon Lex and Amazon Kendra to provide the conversational intent matching, context capture, and knowledge base search capabilities used for Agent Assist.
    - KENDRA - Amazon Kendra is an intelligent enterprise search service that allows users to search across different content repositories with built-in connectors.
    - AISTACK - These are the lambda functions shown in the diagram on the introduction page. 
2. Set up AudioHook - AudioHook is used to stream conversation audio to AWS in this use case. 




