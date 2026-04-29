---
description: A single message in a chat conversation
layout: schema
name: Message
properties_list:
- description: 'Message role: system, user, assistant, tool'
  name: role
  type: string
- description: Message content text
  name: content
  type: string
- description: Optional name for the participant
  name: name
  type: string
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-message-schema.json
slug: aimlapi-message
source_filename: aimlapi-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"A single message in a chat conversation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Message role: system, user, assistant, tool\",\n      \"example\": \"user\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Message content text\",\n      \"example\": \"Hello, how can I help you?\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional name for the participant\",\n      \"example\": \"Alice\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-message-schema.json
tags:
- Artificial Intelligence
- Machine Learning
- AI Models
- LLM
- Image Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
title: Message
---
