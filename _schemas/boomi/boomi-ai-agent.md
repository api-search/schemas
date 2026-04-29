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
source_filename: boomi-ai-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.boomi.com/schemas/ai-agent.json\",\n  \"title\": \"Boomi AI Agent\",\n  \"description\": \"Represents a Boomi AI agent managed through Boomi Agentstudio — an entity that uses large language models to autonomously handle tasks, orchestrate integrations, and respond to user requests. Agents are configured with tools, guardrails, and LLM provider settings via the Agent Control Tower.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the AI agent.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the AI agent.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the agent's purpose and capabilities.\"\
  \n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Boomi account ID that owns this agent.\"\n    },\n    \"providerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the external AI provider if this agent is from a third-party system.\"\n    },\n    \"providerType\": {\n      \"type\": \"string\",\n      \"description\": \"The AI provider powering this agent.\",\n      \"enum\": [\"BOOMI\", \"AMAZON_BEDROCK\", \"CUSTOM\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state of the agent.\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"DEPLOYING\", \"ERROR\"]\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"Tools (API endpoints, integrations) available to this agent.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AgentTool\"\n      }\n    },\n    \"guardrails\": {\n      \"type\": \"array\",\n      \"description\": \"Guardrail configurations controlling\
  \ the agent's behavior boundaries.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Guardrail\"\n      }\n    },\n    \"llmConfig\": {\n      \"$ref\": \"#/$defs/LLMConfig\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the agent was created.\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the agent was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"AgentTool\": {\n      \"type\": \"object\",\n      \"title\": \"Agent Tool\",\n      \"description\": \"A tool available to a Boomi AI agent — an API endpoint or integration that the agent can invoke to take action.\",\n      \"required\": [\"id\", \"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the tool.\"\n        },\n        \"name\": {\n     \
  \     \"type\": \"string\",\n          \"description\": \"Display name of the tool shown to the agent.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description that helps the agent understand when and how to use this tool.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of tool.\",\n          \"enum\": [\"API_ENDPOINT\", \"BOOMI_PROCESS\", \"MCP_SERVER\", \"FUNCTION\"]\n        },\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the API endpoint or MCP server this tool points to.\"\n        },\n        \"authentication\": {\n          \"$ref\": \"#/$defs/ToolAuthentication\"\n        },\n        \"inputSchema\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema describing the expected input parameters for this tool.\",\n          \"additionalProperties\": true\n       \
  \ },\n        \"outputSchema\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema describing the expected output of this tool.\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"ToolAuthentication\": {\n      \"type\": \"object\",\n      \"title\": \"Tool Authentication\",\n      \"description\": \"Authentication configuration for connecting an agent tool to an external service.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Authentication mechanism.\",\n          \"enum\": [\"BEARER_TOKEN\", \"API_KEY\", \"OAUTH2\", \"BASIC\", \"NONE\"]\n        },\n        \"tokenSource\": {\n          \"type\": \"string\",\n          \"description\": \"Where the token or credential is sourced from.\",\n          \"enum\": [\"ENVIRONMENT_VARIABLE\", \"BOOMI_CONNECTION\", \"DELEGATED_USER\"]\n        },\n        \"connectionId\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"ID of the Boomi connection providing credentials, if applicable.\"\n        }\n      }\n    },\n    \"Guardrail\": {\n      \"type\": \"object\",\n      \"title\": \"Guardrail\",\n      \"description\": \"A safety constraint applied to an AI agent to control its behavior and output.\",\n      \"required\": [\"id\", \"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the guardrail.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of guardrail constraint.\",\n          \"enum\": [\"CONTENT_FILTER\", \"TOPIC_RESTRICTION\", \"RATE_LIMIT\", \"PII_FILTER\", \"HALLUCINATION_DETECTION\"]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the guardrail.\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"description\": \"\
  Guardrail-specific configuration parameters.\",\n          \"additionalProperties\": true\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this guardrail is currently active.\"\n        }\n      }\n    },\n    \"LLMConfig\": {\n      \"type\": \"object\",\n      \"title\": \"LLM Configuration\",\n      \"description\": \"Configuration for the large language model powering an AI agent.\",\n      \"required\": [\"provider\"],\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"The LLM provider.\",\n          \"enum\": [\"AMAZON_BEDROCK\", \"OPENAI\", \"ANTHROPIC\", \"CUSTOM\"]\n        },\n        \"modelId\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the specific model to use (e.g., anthropic.claude-3-sonnet).\"\n        },\n        \"temperature\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\"\
  : 1,\n          \"description\": \"Sampling temperature controlling response randomness (0 = deterministic, 1 = creative).\"\n        },\n        \"maxTokens\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum number of tokens to generate in a response.\"\n        },\n        \"systemPrompt\": {\n          \"type\": \"string\",\n          \"description\": \"System-level instructions that define the agent's persona and behavior.\"\n        },\n        \"credentials\": {\n          \"$ref\": \"#/$defs/ToolAuthentication\"\n        }\n      }\n    },\n    \"AgentTask\": {\n      \"type\": \"object\",\n      \"title\": \"Agent Task\",\n      \"description\": \"A task submitted to a Boomi AI agent for execution.\",\n      \"required\": [\"id\", \"agentId\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the task.\"\n        },\n        \"agentId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"ID of the agent assigned to execute this task.\"\n        },\n        \"input\": {\n          \"type\": \"string\",\n          \"description\": \"Natural language or structured input describing the task.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current execution status of the task.\",\n          \"enum\": [\"PENDING\", \"RUNNING\", \"COMPLETED\", \"FAILED\", \"CANCELLED\"]\n        },\n        \"output\": {\n          \"type\": \"string\",\n          \"description\": \"The agent's response or result after completing the task.\"\n        },\n        \"toolCalls\": {\n          \"type\": \"array\",\n          \"description\": \"Record of tool invocations made by the agent during task execution.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"toolId\": {\n                \"type\": \"string\",\n         \
  \       \"description\": \"ID of the tool that was called.\"\n              },\n              \"input\": {\n                \"type\": \"object\",\n                \"description\": \"Input parameters passed to the tool.\",\n                \"additionalProperties\": true\n              },\n              \"output\": {\n                \"type\": \"object\",\n                \"description\": \"Output returned by the tool.\",\n                \"additionalProperties\": true\n              },\n              \"timestamp\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"When the tool was invoked.\"\n              }\n            }\n          }\n        },\n        \"createdDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the task was submitted.\"\n        },\n        \"completedDate\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the task completed.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/json-schema/boomi-ai-agent-schema.json
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
