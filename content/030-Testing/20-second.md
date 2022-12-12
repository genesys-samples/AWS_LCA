---
title: "Explore Agent Assist Features"
chapter: false
weight: 20
---

## Explore Agent Assist Features
Our Agent Assist capabilities are enabled using [QnABot on AWS](https://aws.amazon.com/solutions/implementations/qnabot-on-aws/). In summary, QnABot will orchestrate Amazon Lex and Amazon Kendra to provide intent matching, context capture, and knowledge base search capabilities used for Agent Assist. In the administrative UI, Content Designer, you can configure how messages are generated for your agents. While there are other options for implementing Agent Assist with AWS, such as integrating your own Amazon Lex Bot or using AWS Lambda Functions, let's check out what the implementation we just set up can do. 

1. Open and Review the [Agent Assist demo script](https://github.com/aws-samples/amazon-transcribe-live-call-analytics/blob/main/lca-agentassist-setup-stack/agent-assist-demo-script.md)
2. Make a phone call to the number that is routing to your Architect flow
3. Play the role of the caller from the demo script dialog
    - It's best to get a friend to play the role of the agent. Your agent friend will use their Genesys Cloud CX softphone to answer your call and speak the lines from the script. If you can't do that, it's okay! You can still test Agent Assist by just playing the role of the caller. 
4. As you say certain phrases in the script, you should see messages labelled AGENT_ASSISTANT as they appear in the transcript in near real time. These messages would help guide the agent to respond to the caller. 

Think about the concepts at work in this example and consider how you could apply them to your own contact center scenarios.

For much further detail on how to customize and extend the capabilities, see our [Agent Assist README](https://github.com/aws-samples/amazon-transcribe-live-call-analytics/blob/main/lca-agentassist-setup-stack/README.md). We plan to add more capabilities to the LCA Agent Assistant in future releases. Please share what features would be important to your business. //note: where would they share this feedback?