---
description: A text content block in a response.
layout: schema
name: TextBlock
properties_list:
- description: ''
  name: type
  type: string
- description: The text content.
  name: text
  type: string
- description: Citations for the text content, if any.
  name: citations
  type: array
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-text-block-schema.json
slug: claude-messages-text-block
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextBlock\",\n  \"type\": \"object\",\n  \"description\": \"A text content block in a response.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content.\"\n    },\n    \"citations\": {\n      \"type\": \"array\",\n      \"description\": \"Citations for the text content, if any.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-text-block-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: TextBlock
---
