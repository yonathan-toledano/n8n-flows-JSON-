# n8n Workflows for AI Agents and Automation

This repository contains production style n8n workflows built for automation, AI agents, and messaging integrations.
All workflows are created using free and self hosted tools, with a focus on practical, real world use cases.

The repository demonstrates how to design end to end AI flows without relying on paid SaaS services.

# Architecture Overview

The repository includes two main AI based workflows, each using a different setup and communication method.

1. Local AI Model using Self Hosted AI Starter Kit

One workflow is based on a locally hosted AI model, deployed using a self hosted AI starter kit.

High level flow:
• The AI model runs locally on the server
• n8n communicates directly with the local model via HTTP
• No external AI providers are required
• Full control over data, prompts, and behavior

This setup is ideal for:
• Privacy sensitive use cases
• Offline or low cost environments
• Experimentation with local LLMs
• Full ownership of the AI stack

The workflow shows how n8n can act as the orchestration layer for a local AI agent, including input handling, routing, and response formatting.

2. AI Workflow using Tunnel and WhatsApp Integration

The second workflow uses an n8n tunnel to expose webhooks publicly and connect the AI logic to WhatsApp messaging.

High level flow:
• Incoming WhatsApp messages are received via webhook
• n8n processes and validates the input
• The request is sent to an AI model endpoint
• The AI response is routed back to WhatsApp
• Includes basic routing and fallback logic

This setup allows:
• Real time AI conversations over WhatsApp
• No need for public hosting or paid infrastructure
• Fast prototyping of conversational agents
• External access using n8n tunnel only

# Cost and Tooling

# Important note:
Both workflows were built entirely using free and self hosted tools.

• n8n self hosted
• Local AI model using an open source starter kit
• n8n tunnel for public access
• No paid AI APIs
• No paid automation platforms

This repository shows that it is possible to build end to end AI powered automation and messaging systems with zero platform cost.

# What This Repository Demonstrates

• Designing AI agent workflows
• Orchestrating local and remote AI models
• Webhook based integrations
• Messaging automation with WhatsApp
• Practical n8n architecture patterns
• Free and self hosted AI systems

# 👤 Author
Yonathan Toledano GitHub: https://github.com/yonathan-toledano using n8n
# Notes

• All workflows are provided as JSON exports
• Credentials and secrets are excluded
• The flows are meant for learning, reuse, and adaptation

