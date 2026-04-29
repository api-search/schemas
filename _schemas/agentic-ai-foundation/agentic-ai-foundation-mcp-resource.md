---
description: A data resource exposed by an MCP server, accessible to AI agent clients for reading context.
layout: schema
name: MCPResource
properties_list:
- description: Unique URI identifying this resource.
  name: uri
  type: string
- description: Human-readable name of the resource.
  name: name
  type: string
- description: Human-readable description of the resource's contents.
  name: description
  type: string
- description: MIME type of the resource content.
  name: mimeType
  type: string
- description: Size of the resource in bytes.
  name: size
  type: integer
provider_name: Agentic AI Foundation
provider_slug: agentic-ai-foundation
schema_file: json-schema/agentic-ai-foundation-mcp-resource-schema.json
slug: agentic-ai-foundation-mcp-resource
source_filename: agentic-ai-foundation-mcp-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/json-schema/agentic-ai-foundation-mcp-resource-schema.json\",\n  \"title\": \"MCPResource\",\n  \"description\": \"A data resource exposed by an MCP server, accessible to AI agent clients for reading context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Unique URI identifying this resource.\",\n      \"example\": \"file:///home/user/documents/report.pdf\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the resource.\",\n      \"example\": \"Quarterly Report\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the resource's contents.\",\n      \"example\": \"Q1 2026 financial report in PDF\
  \ format.\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the resource content.\",\n      \"example\": \"application/pdf\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the resource in bytes.\",\n      \"example\": 204800\n    }\n  },\n  \"required\": [\"uri\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/json-schema/agentic-ai-foundation-mcp-resource-schema.json
tags:
- AI Agents
- Linux Foundation
- Open Source
- Standards
- MCP
- Agentic AI
- Interoperability
title: MCPResource
---
