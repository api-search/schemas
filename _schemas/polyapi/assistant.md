---
description: An AI assistant conversation for AI-powered document assistance and discovery in PolyAPI.
layout: schema
name: PolyAPI Assistant Conversation
properties_list:
- description: The unique identifier of the conversation.
  name: id
  type: string
- description: The slug identifier for the conversation.
  name: slug
  type: string
- description: The list of messages in the conversation.
  name: messages
  type: array
- description: Timestamp when the conversation was created.
  name: createdAt
  type: string
- description: Timestamp when the conversation was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/assistant.json
slug: assistant
source_filename: assistant.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/assistant.json\",\n  \"title\": \"PolyAPI Assistant Conversation\",\n  \"description\": \"An AI assistant conversation for AI-powered document assistance and discovery in PolyAPI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the conversation.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The slug identifier for the conversation.\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"role\": {\n            \"type\": \"string\",\n            \"enum\": [\"user\", \"assistant\"],\n            \"description\": \"The role of the message sender.\"\n          },\n          \"content\": {\n            \"type\": \"\
  string\",\n            \"description\": \"The message content.\"\n          }\n        }\n      },\n      \"description\": \"The list of messages in the conversation.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the conversation was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the conversation was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/assistant.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Assistant Conversation
---
