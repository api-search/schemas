---
description: Configuration for extended thinking.
layout: schema
name: ThinkingConfig
properties_list:
- description: Whether thinking is enabled, disabled, or adaptive.
  name: type
  type: string
- description: Maximum number of tokens for thinking. Minimum 1024 and must be less than max_tokens.
  name: budget_tokens
  type: integer
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-thinking-config-schema.json
slug: claude-messages-thinking-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThinkingConfig\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for extended thinking.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Whether thinking is enabled, disabled, or adaptive.\"\n    },\n    \"budget_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of tokens for thinking. Minimum 1024 and must be less than max_tokens.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-thinking-config-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ThinkingConfig
---
