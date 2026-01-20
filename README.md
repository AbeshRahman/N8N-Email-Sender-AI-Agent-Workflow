# N8N-Email-Sender-AI-Agent

This repository contains an AI-powered email automation workflow built using **n8n**.  
The workflow allows users to send emails by providing instructions through a chat interface, where an AI agent generates and sends the email automatically using Gmail.

This project is intended for demonstration, learning, and portfolio purposes.

Below is the visual representation of the complete workflow:

![Email Sender AI Agent Workflow](https://github.com/AbeshRahman/N8N-Email-Sender-AI-Agent-Workflow/blob/main/Email%20Sender%20AI%20Agent%20Workflow.png)

## Workflow Description

The workflow begins when a message is received through n8n’s built-in chat interface. This chat message acts as the trigger for the automation.

Once triggered, the message is passed to an **AI Agent** node. The AI Agent acts as the central controller of the workflow and coordinates multiple components to complete the task.

The agent uses **Google Gemini Chat Model** to understand the user’s input and generate structured email content, including the recipient, subject line, and email body.

To maintain conversational context, the AI Agent is connected to a **Simple Memory** node. This allows the agent to remember recent messages within the same session, enabling more natural and consistent interactions.

After generating the email content, the AI Agent invokes the **Gmail tool** to send the email. The recipient address, subject, and message body are dynamically populated using AI-generated values at runtime.

The entire process—from user instruction to email delivery—happens automatically without any manual drafting.

## Included Files

The `workflows` folder contains the exported **n8n workflow JSON file**, which represents the complete automation logic.

The `screenshots` folder contains images of the workflow for easy visual understanding.

## How to Use the Workflow

Download the workflow JSON file from the `workflows` folder.

Open your n8n editor and select **Import from file**.

After importing, configure the required credentials such as Google Gemini API and Gmail OAuth.

Once configured, open the chat interface and start sending instructions to generate and send emails.

## Logs, Chatbot & Automated Email sent 

![Email Sender AI Agent Workflow](https://github.com/AbeshRahman/N8N-Email-Sender-AI-Agent-Workflow/blob/main/Chatbot%20%26%20Logs%20Overview.png)
![Email Sender AI Agent Workflow](https://github.com/AbeshRahman/N8N-Email-Sender-AI-Agent-Workflow/blob/main/Automated%20Email%20Sent%20by%20N8N.png)
