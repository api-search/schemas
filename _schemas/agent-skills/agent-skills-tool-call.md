---
description: An AI agent's invocation of a tool skill with specific input parameters.
layout: schema
name: ToolCall
properties_list:
- description: Unique identifier for this tool call instance.
  name: id
  type: string
- description: Content block type, always tool_use.
  name: type
  type: string
- description: Name of the tool being called.
  name: name
  type: string
- description: Input parameters provided to the tool, conforming to the tool's input_schema.
  name: input
  type: object
provider_name: Agent Skills
provider_slug: agent-skills
schema_file: json-schema/agent-skills-tool-call-schema.json
slug: agent-skills-tool-call
source_filename: agent-skills-tool-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-tool-call-schema.json\",\n  \"title\": \"ToolCall\",\n  \"description\": \"An AI agent's invocation of a tool skill with specific input parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this tool call instance.\",\n      \"example\": \"toolu_01A09q90qw90lq917835lq9\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Content block type, always tool_use.\",\n      \"example\": \"tool_use\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the tool being called.\",\n      \"example\": \"get_weather\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters provided to the tool, conforming\
  \ to the tool's input_schema.\",\n      \"example\": { \"location\": \"San Francisco, CA\" }\n    }\n  },\n  \"required\": [\"id\", \"type\", \"name\", \"input\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/json-schema/agent-skills-tool-call-schema.json
tags:
- Agent Skills
- AI Agents
- Tool Use
- Function Calling
- MCP
- Agentic AI
- Automation
title: ToolCall
---
