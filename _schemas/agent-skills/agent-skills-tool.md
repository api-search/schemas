---
description: A skill definition for an AI agent including name, description, and input parameter schema.
layout: schema
name: Tool
properties_list:
- description: The type of tool (custom or provider built-in).
  name: type
  type: string
- description: Unique name of the tool used to identify the invocation.
  name: name
  type: string
- description: Human-readable description of what the tool does, used by the model to decide when to call it.
  name: description
  type: string
- description: JSON Schema defining the parameters the tool accepts.
  name: input_schema
  type: object
- description: When true, enforces strict JSON Schema compliance for tool call inputs.
  name: strict
  type: boolean
provider_name: Agent Skills
provider_slug: agent-skills
schema_file: json-schema/agent-skills-tool-schema.json
slug: agent-skills-tool
source_filename: agent-skills-tool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-tool-schema.json\",\n  \"title\": \"Tool\",\n  \"description\": \"A skill definition for an AI agent including name, description, and input parameter schema.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of tool (custom or provider built-in).\",\n      \"example\": \"function\",\n      \"enum\": [\"function\", \"web_search_20260209\", \"code_execution_20260209\", \"web_fetch_20260209\", \"tool_search_20260209\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the tool used to identify the invocation.\",\n      \"example\": \"get_weather\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what the tool\
  \ does, used by the model to decide when to call it.\",\n      \"example\": \"Get the current weather for a given location.\"\n    },\n    \"input_schema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema defining the parameters the tool accepts.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"object\"\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\": \"Map of parameter names to their schema definitions.\"\n        },\n        \"required\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"List of required parameter names.\"\n        }\n      }\n    },\n    \"strict\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, enforces strict JSON Schema compliance for tool call inputs.\",\n      \"example\": false\n    }\n  },\n  \"required\": [\"name\", \"description\", \"input_schema\"\
  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-tool-schema.json
tags:
- Agent Skills
- AI Agents
- Tool Use
- Function Calling
- MCP
- Agentic AI
- Automation
title: Tool
---
