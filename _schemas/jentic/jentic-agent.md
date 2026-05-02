---
description: Represents an AI agent configured on the Jentic platform, including its scoped API access, credentials, and API key configuration.
layout: schema
name: Jentic Agent
properties_list:
- description: Human-readable name for the agent.
  name: name
  type: string
- description: Description of the agent's purpose and capabilities.
  name: description
  type: string
- description: The scoped API key for this agent, used in the X-JENTIC-API-KEY header.
  name: api_key
  type: string
- description: List of API identifiers this agent is permitted to access.
  name: allowed_apis
  type: array
- description: List of workflow identifiers this agent is permitted to execute.
  name: allowed_workflows
  type: array
- description: Upstream API credentials assigned to this agent, stored encrypted in the Jentic credential vault.
  name: credentials
  type: array
- description: Rate limiting configuration for this agent.
  name: rate_limit
  type: object
- description: Timestamp when the agent was created.
  name: created_at
  type: string
- description: Timestamp when the agent was last updated.
  name: updated_at
  type: string
provider_name: Jentic
provider_slug: jentic
schema_file: json-schema/jentic-agent-schema.json
slug: jentic-agent
source_filename: jentic-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jentic.com/schemas/jentic/agent.json\",\n  \"title\": \"Jentic Agent\",\n  \"description\": \"Represents an AI agent configured on the Jentic platform, including its scoped API access, credentials, and API key configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the agent.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the agent's purpose and capabilities.\"\n    },\n    \"api_key\": {\n      \"type\": \"string\",\n      \"description\": \"The scoped API key for this agent, used in the X-JENTIC-API-KEY header.\"\n    },\n    \"allowed_apis\": {\n      \"type\": \"array\",\n      \"description\": \"List of API identifiers this agent is permitted to access.\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"allowed_workflows\": {\n      \"type\": \"array\",\n      \"description\": \"List of workflow identifiers this agent is permitted to execute.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"credentials\": {\n      \"type\": \"array\",\n      \"description\": \"Upstream API credentials assigned to this agent, stored encrypted in the Jentic credential vault.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CredentialReference\"\n      }\n    },\n    \"rate_limit\": {\n      \"$ref\": \"#/$defs/RateLimit\",\n      \"description\": \"Rate limiting configuration for this agent.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the agent was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the agent was last updated.\"\n \
  \   }\n  },\n  \"$defs\": {\n    \"CredentialReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to an encrypted credential stored in the Jentic vault for a specific upstream API.\",\n      \"required\": [\"api_name\", \"credential_type\"],\n      \"properties\": {\n        \"api_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the upstream API this credential authenticates with.\"\n        },\n        \"credential_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of credential stored.\",\n          \"enum\": [\"api_key\", \"oauth2\", \"basic\", \"bearer_token\"]\n        },\n        \"credential_id\": {\n          \"type\": \"string\",\n          \"description\": \"Internal identifier for the stored credential in the vault.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the credential.\",\n          \"enum\": [\"active\", \"\
  expired\", \"revoked\"]\n        }\n      }\n    },\n    \"RateLimit\": {\n      \"type\": \"object\",\n      \"description\": \"Rate limiting configuration for agent API requests.\",\n      \"properties\": {\n        \"requests_per_minute\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of requests allowed per minute.\",\n          \"minimum\": 1\n        },\n        \"requests_per_day\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of requests allowed per day.\",\n          \"minimum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jentic/refs/heads/main/json-schema/jentic-agent-schema.json
tags:
- AI Agents
- Arazzo
- Integrations
- MCP
- OpenAPI
- Workflows
title: Jentic Agent
---
