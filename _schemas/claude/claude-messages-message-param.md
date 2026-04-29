---
description: An input message in the conversation.
layout: schema
name: MessageParam
properties_list:
- description: The role of the message author.
  name: role
  type: string
- description: The content of the message. Can be a string or array of content blocks.
  name: content
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-message-param-schema.json
slug: claude-messages-message-param
source_filename: claude-messages-message-param-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageParam\",\n  \"type\": \"object\",\n  \"description\": \"An input message in the conversation.\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the message author.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the message. Can be a string or array of content blocks.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-message-param-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: MessageParam
---
