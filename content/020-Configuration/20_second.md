---
title: "Set up AudioHook"
chapter: false
weight: 20
---

## Set up AudioHook
The next step of the process is to configure AudioHook. Audiohook will stream audio to our CloudFront web socket endpoint. Please refer to the diagram on the Solution Overview page if you want to review the architecture of what AWS is doing with the audio stream.

To configure Audiohook in Genesys Cloud CX, follow these steps: 

1. Navigate to the Admin Console and then to Integrations 
2. Click to add integration and then select AudioHook
3. Click to install the integration, give it a descriptive name and then navigate to the Configuration > Properties tab.
    - For the Channel selection, choose "Both"
4. To get the Connection URI, navigate back to AWS > search for Cloudfront > Stacks > Choose the "LCA" Stack > and then click on Outputs > find the "WebSocketEndpoint" value
![Web Socket Endpoint](/images/webSocketEndpoint.jpg)
    - Copy and paste this value back into the Connection URI field in your AudioHook integration
5. In the AudioHook integration configuration, navigate to Credentials
6. To get the API Key and Client Secret, navigate back to AWS > Secrets Manager > Click on the secret that ends in API key > Click on Retrieve secret value
    - copy this value into the corresponding Credentials field in Genesys Cloud CX
    - Repeat the step for the Client secret
    ![Secret](/images/secret.jpg)
7. Press save and Activate the integration! 