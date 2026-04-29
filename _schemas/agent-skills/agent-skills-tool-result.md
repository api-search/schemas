---
description: The output returned to an AI agent after executing a tool skill.
layout: schema
name: ToolResult
properties_list:
- description: Content block type, always tool_result.
  name: type
  type: string
- description: The id of the tool_use block this result corresponds to.
  name: tool_use_id
  type: string
- description: The result content returned from the tool. Can be a string or array of content blocks.
  name: content
  type: object
- description: When true, indicates the tool execution returned an error.
  name: is_error
  type: boolean
provider_name: Agent Skills
provider_slug: agent-skills
schema_file: json-schema/agent-skills-tool-result-schema.json
slug: agent-skills-tool-result
source_filename: agent-skills-tool-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-tool-result-schema.json\",\n  \"title\": \"ToolResult\",\n  \"description\": \"The output returned to an AI agent after executing a tool skill.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Content block type, always tool_result.\",\n      \"example\": \"tool_result\"\n    },\n    \"tool_use_id\": {\n      \"type\": \"string\",\n      \"description\": \"The id of the tool_use block this result corresponds to.\",\n      \"example\": \"toolu_01A09q90qw90lq917835lq9\"\n    },\n    \"content\": {\n      \"description\": \"The result content returned from the tool. Can be a string or array of content blocks.\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        {\n          \"type\": \"array\",\n          \"items\"\
  : {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": { \"type\": \"string\" },\n              \"text\": { \"type\": \"string\" }\n            }\n          }\n        }\n      ],\n      \"example\": \"72°F and sunny in San Francisco, CA\"\n    },\n    \"is_error\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, indicates the tool execution returned an error.\",\n      \"example\": false\n    }\n  },\n  \"required\": [\"type\", \"tool_use_id\", \"content\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-tool-result-schema.json
tags:
- Agent Skills
- AI Agents
- Tool Use
- Function Calling
- MCP
- Agentic AI
- Automation
title: ToolResult
---
