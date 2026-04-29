---
description: How the model should use the provided tools.
layout: schema
name: ToolChoice
properties_list:
- description: The type of tool choice. "auto" lets the model decide, "any" forces tool use, "tool" forces a specific tool, "none" disables tools.
  name: type
  type: string
- description: The name of the tool to use. Required when type is "tool".
  name: name
  type: string
- description: Whether to disable parallel tool use.
  name: disable_parallel_tool_use
  type: boolean
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-tool-choice-schema.json
slug: claude-messages-tool-choice
source_filename: claude-messages-tool-choice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolChoice\",\n  \"type\": \"object\",\n  \"description\": \"How the model should use the provided tools.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of tool choice. \\\"auto\\\" lets the model decide, \\\"any\\\" forces tool use, \\\"tool\\\" forces a specific tool, \\\"none\\\" disables tools.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tool to use. Required when type is \\\"tool\\\".\"\n    },\n    \"disable_parallel_tool_use\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable parallel tool use.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-tool-choice-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ToolChoice
---
