---
description: Conversation schema from openapi
layout: schema
name: Conversation
properties_list:
- description: The unique identifier of the conversation.
  name: conversationId
  type: string
- description: The title of the conversation.
  name: title
  type: string
- description: The date and time the conversation was created.
  name: createdAt
  type: string
provider_name: Amazon Q
provider_slug: amazon-q
schema_file: json-schema/amazon-q-openapi-conversation-schema.json
slug: amazon-q-openapi-conversation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-conversation-schema.json\",\n  \"title\": \"Conversation\",\n  \"description\": \"Conversation schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conversationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the conversation.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the conversation.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the conversation was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-conversation-schema.json
tags:
- Artificial Intelligence
- Assistant
- AWS
- Enterprise
- Generative AI
title: Conversation
---
