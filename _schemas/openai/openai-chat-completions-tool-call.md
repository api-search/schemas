---
description: ''
layout: schema
name: ToolCall
properties_list:
- description: The ID of the tool call.
  name: id
  type: string
- description: The type of the tool call.
  name: type
  type: string
- description: ''
  name: function
  type: object
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-chat-completions-tool-call-schema.json
slug: openai-chat-completions-tool-call
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolCall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the tool call.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the tool call.\"\n    },\n    \"function\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-chat-completions-tool-call-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: ToolCall
---
