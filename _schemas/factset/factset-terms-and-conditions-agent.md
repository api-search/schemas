---
description: Agent Data Items for a Fixed Income security.
layout: schema
name: agent
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: FactSet Entity Identifier for the Agent.
  name: agentEntityId
  type: string
- description: Agent Commitment Amount
  name: agentCommAmt
  type: number
- description: Agent Name
  name: agentName
  type: string
- description: Role of the agent
  name: agentType
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-agent-schema.json
slug: factset-terms-and-conditions-agent
source_filename: factset-terms-and-conditions-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"agent\",\n  \"type\": \"object\",\n  \"description\": \"Agent Data Items for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"agentEntityId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier for the Agent.\"\n    },\n    \"agentCommAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Agent Commitment Amount\"\n    },\n    \"agentName\": {\n      \"type\": \"string\",\n      \"description\": \"Agent Name\"\n    },\n    \"agentType\": {\n      \"type\": \"string\",\n      \"description\": \"Role of the agent\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-agent-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: agent
---
