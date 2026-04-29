---
description: ''
layout: schema
name: TokenCount
properties_list:
- description: The total number of input tokens in the message.
  name: input_tokens
  type: integer
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-token-count-schema.json
slug: claude-messages-token-count
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TokenCount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of input tokens in the message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-token-count-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: TokenCount
---
