---
description: Represents a Boomi AI agent managed through Boomi Agentstudio — an entity that uses large language models to autonomously handle tasks, orchestrate integrations, and respond to user requests. Agents are configured with tools, guardrails, and LLM provider settings via the Agent Control Tower.
layout: schema
name: Boomi AI Agent
properties_list:
- description: Unique identifier of the AI agent.
  name: id
  type: string
- description: Display name of the AI agent.
  name: name
  type: string
- description: Human-readable description of the agent's purpose and capabilities.
  name: description
  type: string
- description: Boomi account ID that owns this agent.
  name: accountId
  type: string
- description: ID of the external AI provider if this agent is from a third-party system.
  name: providerId
  type: string
- description: The AI provider powering this agent.
  name: providerType
  type: string
- description: Current operational state of the agent.
  name: state
  type: string
- description: Tools (API endpoints, integrations) available to this agent.
  name: tools
  type: array
- description: Guardrail configurations controlling the agent's behavior boundaries.
  name: guardrails
  type: array
- description: ''
  name: llmConfig
  type: object
- description: ISO 8601 timestamp when the agent was created.
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the agent was last modified.
  name: modifiedDate
  type: string
provider_name: Boomi
provider_slug: boomi
schema_file: json-schema/boomi-ai-agent-schema.json
slug: boomi-ai-agent
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integrations
- Management
- MFT
- Platform
- Workflows
title: Boomi AI Agent
---
