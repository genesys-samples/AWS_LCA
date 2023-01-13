---
title: "Configuration"
chapter: true
weight: 20
---

## Configuration
**The configuration of this integration is broken up into two parts.** 

### 1. Deploy the CloudFormation Stack in AWS - In this section, we will walk you through deploying a CloudFormation Stack in AWS. The CloudFormation will deploy 3 main components: 
- #### **QNABOT** - QnABot conveniently orchestrates Amazon Lex and Amazon Kendra to provide the conversational intent matching, context capture, and knowledge base search capabilities used for Agent Assist.
- #### **KENDRA** - Amazon Kendra is an intelligent enterprise search service that allows users to search across different content repositories with built-in connectors.
- #### **AISTACK** - These are the lambda functions shown in the diagram on the introduction page. 
- #### **Cloudformation** - AWS CloudFormation is a service that gives developers and businesses an easy way to create a collection of related AWS and third-party resources, and provision and manage them in an orderly and predictable fashion.
- #### **Amazon Lex** - Amazon Lex is an AWS service for building conversational interfaces for applications using voice and text. With Amazon Lex, the same conversational engine that powers Amazon Alexa is now available to any developer, enabling you to build sophisticated, natural language chatbots into your new and existing applications. Amazon Lex provides the deep functionality and flexibility of natural language understanding (NLU) and automatic speech recognition (ASR) so you can build highly engaging user experiences with lifelike, conversational interactions, and create new categories of products.
### 2. Set up AudioHook - AudioHook is used to stream conversation audio to AWS in this use case. 




