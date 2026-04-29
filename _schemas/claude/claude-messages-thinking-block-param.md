---
description: A thinking content block in a request (for multi-turn with extended thinking).
layout: schema
name: ThinkingBlockParam
properties_list:
- description: ''
  name: type
  type: string
- description: The thinking text from a previous response.
  name: thinking
  type: string
- description: The signature from the previous thinking block.
  name: signature
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-thinking-block-param-schema.json
slug: claude-messages-thinking-block-param
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThinkingBlockParam\",\n  \"type\": \"object\",\n  \"description\": \"A thinking content block in a request (for multi-turn with extended thinking).\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"thinking\": {\n      \"type\": \"string\",\n      \"description\": \"The thinking text from a previous response.\"\n    },\n    \"signature\": {\n      \"type\": \"string\",\n      \"description\": \"The signature from the previous thinking block.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-thinking-block-param-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ThinkingBlockParam
---
