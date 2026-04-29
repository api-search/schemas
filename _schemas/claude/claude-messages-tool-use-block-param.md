---
description: A tool use content block in a request (for multi-turn tool use).
layout: schema
name: ToolUseBlockParam
properties_list:
- description: ''
  name: type
  type: string
- description: The unique identifier for this tool use.
  name: id
  type: string
- description: The name of the tool.
  name: name
  type: string
- description: The input to the tool.
  name: input
  type: object
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-tool-use-block-param-schema.json
slug: claude-messages-tool-use-block-param
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolUseBlockParam\",\n  \"type\": \"object\",\n  \"description\": \"A tool use content block in a request (for multi-turn tool use).\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this tool use.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tool.\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"The input to the tool.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-tool-use-block-param-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ToolUseBlockParam
---
