---
description: An MCP tool definition exposed by an MCP server, discoverable by AI agent clients.
layout: schema
name: MCPTool
properties_list:
- description: Unique name of the tool.
  name: name
  type: string
- description: Human-readable description of what the tool does.
  name: description
  type: string
- description: JSON Schema defining the tool's input parameters.
  name: inputSchema
  type: object
- description: Optional metadata annotations for the tool.
  name: annotations
  type: object
provider_name: Agentic AI Foundation
provider_slug: agentic-ai-foundation
schema_file: json-schema/agentic-ai-foundation-mcp-tool-schema.json
slug: agentic-ai-foundation-mcp-tool
source_filename: agentic-ai-foundation-mcp-tool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/json-schema/agentic-ai-foundation-mcp-tool-schema.json\",\n  \"title\": \"MCPTool\",\n  \"description\": \"An MCP tool definition exposed by an MCP server, discoverable by AI agent clients.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the tool.\",\n      \"example\": \"read_file\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what the tool does.\",\n      \"example\": \"Read the contents of a file at the specified path.\"\n    },\n    \"inputSchema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema defining the tool's input parameters.\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"example\": \"object\"\
  \ },\n        \"properties\": { \"type\": \"object\" },\n        \"required\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      }\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"Optional metadata annotations for the tool.\",\n      \"properties\": {\n        \"readOnly\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the tool only reads data and does not modify state.\"\n        },\n        \"destructive\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the tool may cause irreversible side effects.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"description\", \"inputSchema\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/json-schema/agentic-ai-foundation-mcp-tool-schema.json
tags:
- AI Agents
- Linux Foundation
- Open Source
- Standards
- MCP
- Agentic AI
- Interoperability
title: MCPTool
---
