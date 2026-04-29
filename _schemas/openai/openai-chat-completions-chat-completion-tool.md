---
description: ''
layout: schema
name: ChatCompletionTool
properties_list:
- description: The type of the tool. Currently, only function is supported.
  name: type
  type: string
- description: ''
  name: function
  type: object
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-chat-completions-chat-completion-tool-schema.json
slug: openai-chat-completions-chat-completion-tool
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionTool\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the tool. Currently, only function is supported.\"\n    },\n    \"function\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-chat-completions-chat-completion-tool-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: ChatCompletionTool
---
