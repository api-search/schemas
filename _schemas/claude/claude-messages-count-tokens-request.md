---
description: ''
layout: schema
name: CountTokensRequest
properties_list:
- description: The model to use for token counting.
  name: model
  type: string
- description: Input messages to count tokens for.
  name: messages
  type: array
- description: System prompt to include in the token count.
  name: system
  type: string
- description: Tool definitions to include in the token count.
  name: tools
  type: array
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-count-tokens-request-schema.json
slug: claude-messages-count-tokens-request
source_filename: claude-messages-count-tokens-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CountTokensRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model to use for token counting.\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"Input messages to count tokens for.\"\n    },\n    \"system\": {\n      \"type\": \"string\",\n      \"description\": \"System prompt to include in the token count.\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"Tool definitions to include in the token count.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-count-tokens-request-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: CountTokensRequest
---
