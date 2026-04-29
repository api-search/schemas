---
description: A single completion choice in the response.
layout: schema
name: ChatChoice
properties_list:
- description: Index of this choice.
  name: index
  type: integer
- description: ''
  name: message
  type: object
- description: Reason the generation stopped.
  name: finish_reason
  type: string
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-choice-schema.json
slug: bifrost-chat-choice
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChatChoice\",\n  \"type\": \"object\",\n  \"description\": \"A single completion choice in the response.\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Index of this choice.\",\n      \"example\": 0\n    },\n    \"message\": {\n      \"$ref\": \"#/components/schemas/ChatMessage\"\n    },\n    \"finish_reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason the generation stopped.\",\n      \"enum\": [\n        \"stop\",\n        \"length\",\n        \"content_filter\"\n      ],\n      \"example\": \"stop\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-chat-choice-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatChoice
---
