---
description: Configuration for an LLM provider backend in AgentGateway, defining the target model, authentication, and routing parameters.
layout: schema
name: LLMBackend
properties_list:
- description: Unique name for this LLM backend.
  name: name
  type: string
- description: The LLM provider for this backend.
  name: provider
  type: string
- description: The model identifier to use for requests.
  name: model
  type: string
- description: Optional alias exposed to clients instead of the actual model name.
  name: alias
  type: string
- description: Base URL for the LLM provider API endpoint.
  name: baseUrl
  type: string
- description: Authentication configuration for this backend.
  name: authentication
  type: object
- description: Load balancing weight for this backend (higher means more traffic).
  name: weight
  type: integer
- description: Failover priority, lower values have higher priority.
  name: priority
  type: integer
provider_name: AgentGateway
provider_slug: agentgateway
schema_file: json-schema/agentgateway-llm-backend-schema.json
slug: agentgateway-llm-backend
source_filename: agentgateway-llm-backend-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/json-schema/agentgateway-llm-backend-schema.json\",\n  \"title\": \"LLMBackend\",\n  \"description\": \"Configuration for an LLM provider backend in AgentGateway, defining the target model, authentication, and routing parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for this LLM backend.\",\n      \"example\": \"openai-gpt4\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The LLM provider for this backend.\",\n      \"enum\": [\"openai\", \"anthropic\", \"gemini\", \"bedrock\", \"azure-openai\", \"ollama\", \"vllm\"],\n      \"example\": \"openai\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model identifier to use for requests.\",\n      \"example\"\
  : \"gpt-4o\"\n    },\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"Optional alias exposed to clients instead of the actual model name.\",\n      \"example\": \"primary-llm\"\n    },\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL for the LLM provider API endpoint.\",\n      \"example\": \"https://api.openai.com/v1\"\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration for this backend.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"bearer\", \"apikey\", \"basic\"],\n          \"example\": \"bearer\"\n        },\n        \"secretRef\": {\n          \"type\": \"string\",\n          \"description\": \"Reference to a secret containing the API key.\",\n          \"example\": \"openai-api-key\"\n        }\n      }\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Load balancing weight for this backend (higher means more traffic).\",\n      \"example\": 100\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Failover priority, lower values have higher priority.\",\n      \"example\": 1\n    }\n  },\n  \"required\": [\"name\", \"provider\", \"model\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/json-schema/agentgateway-llm-backend-schema.json
tags:
- AI Gateway
- API Gateway
- MCP
- LLM
- Agent-to-Agent
- Open Source
- CNCF
- Observability
- Security
title: LLMBackend
---
