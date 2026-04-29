---
description: Configuration for an MCP server target in AgentGateway, defining a connected MCP tool provider.
layout: schema
name: MCPTarget
properties_list:
- description: Unique name for this MCP target.
  name: name
  type: string
- description: The connection type for this MCP target.
  name: type
  type: string
- description: URL of the MCP server endpoint.
  name: url
  type: string
- description: Authentication configuration for connecting to this MCP server.
  name: authentication
  type: object
- description: List of tool names exposed by this MCP target (empty means all tools are available).
  name: tools
  type: array
- description: List of client identifiers permitted to use this MCP target.
  name: allowedClients
  type: array
provider_name: AgentGateway
provider_slug: agentgateway
schema_file: json-schema/agentgateway-mcp-target-schema.json
slug: agentgateway-mcp-target
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/json-schema/agentgateway-mcp-target-schema.json\",\n  \"title\": \"MCPTarget\",\n  \"description\": \"Configuration for an MCP server target in AgentGateway, defining a connected MCP tool provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for this MCP target.\",\n      \"example\": \"filesystem-tools\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The connection type for this MCP target.\",\n      \"enum\": [\"sse\", \"stdio\", \"http\"],\n      \"example\": \"http\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the MCP server endpoint.\",\n      \"example\": \"http://localhost:3001/mcp\"\n    },\n    \"authentication\": {\n \
  \     \"type\": \"object\",\n      \"description\": \"Authentication configuration for connecting to this MCP server.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"bearer\", \"apikey\", \"none\"],\n          \"example\": \"bearer\"\n        },\n        \"tokenRef\": {\n          \"type\": \"string\",\n          \"description\": \"Reference to the secret containing the authentication token.\",\n          \"example\": \"mcp-server-token\"\n        }\n      }\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"List of tool names exposed by this MCP target (empty means all tools are available).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"read_file\", \"write_file\", \"list_directory\"]\n    },\n    \"allowedClients\": {\n      \"type\": \"array\",\n      \"description\": \"List of client identifiers permitted to use this MCP target.\",\n      \"items\": {\n    \
  \    \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/json-schema/agentgateway-mcp-target-schema.json
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
title: MCPTarget
---
