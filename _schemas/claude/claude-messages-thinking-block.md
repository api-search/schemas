---
description: A thinking content block showing Claude's internal reasoning process.
layout: schema
name: ThinkingBlock
properties_list:
- description: ''
  name: type
  type: string
- description: Claude's internal reasoning text.
  name: thinking
  type: string
- description: A signature verifying the thinking block.
  name: signature
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-thinking-block-schema.json
slug: claude-messages-thinking-block
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThinkingBlock\",\n  \"type\": \"object\",\n  \"description\": \"A thinking content block showing Claude's internal reasoning process.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"thinking\": {\n      \"type\": \"string\",\n      \"description\": \"Claude's internal reasoning text.\"\n    },\n    \"signature\": {\n      \"type\": \"string\",\n      \"description\": \"A signature verifying the thinking block.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-thinking-block-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ThinkingBlock
---
