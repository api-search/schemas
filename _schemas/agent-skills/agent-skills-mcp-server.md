---
description: A Model Context Protocol server that exposes agent skills (tools, resources, prompts) to AI clients.
layout: schema
name: MCPServer
properties_list:
- description: Name of the MCP server.
  name: name
  type: string
- description: Server version.
  name: version
  type: string
- description: Communication transport used by the server.
  name: transport
  type: string
- description: List of tools exposed by this MCP server.
  name: tools
  type: array
- description: List of resources (data sources) the server can provide.
  name: resources
  type: array
- description: Reusable prompt templates exposed by the server.
  name: prompts
  type: array
provider_name: Agent Skills
provider_slug: agent-skills
schema_file: json-schema/agent-skills-mcp-server-schema.json
slug: agent-skills-mcp-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-mcp-server-schema.json\",\n  \"title\": \"MCPServer\",\n  \"description\": \"A Model Context Protocol server that exposes agent skills (tools, resources, prompts) to AI clients.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the MCP server.\",\n      \"example\": \"filesystem-server\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Server version.\",\n      \"example\": \"1.0.0\"\n    },\n    \"transport\": {\n      \"type\": \"string\",\n      \"description\": \"Communication transport used by the server.\",\n      \"enum\": [\"http\", \"stdio\", \"websocket\"],\n      \"example\": \"http\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"List of\
  \ tools exposed by this MCP server.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"description\": { \"type\": \"string\" },\n          \"inputSchema\": { \"type\": \"object\" }\n        }\n      }\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of resources (data sources) the server can provide.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uri\": { \"type\": \"string\", \"format\": \"uri\" },\n          \"name\": { \"type\": \"string\" },\n          \"mimeType\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"prompts\": {\n      \"type\": \"array\",\n      \"description\": \"Reusable prompt templates exposed by the server.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"description\": { \"type\": \"string\"\
  \ }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"transport\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-mcp-server-schema.json
tags:
- Agent Skills
- AI Agents
- Tool Use
- Function Calling
- MCP
- Agentic AI
- Automation
title: MCPServer
---
