---
description: ''
layout: schema
name: ResponseInputItemList
properties_list:
- description: The object type.
  name: object
  type: string
- description: The list of input items.
  name: data
  type: array
- description: Whether there are more items to retrieve.
  name: has_more
  type: boolean
- description: The ID of the first item in the list.
  name: first_id
  type: string
- description: The ID of the last item in the list.
  name: last_id
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-input-item-list-schema.json
slug: chatgpt-responses-response-input-item-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseInputItemList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of input items.\"\n    },\n    \"has_more\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there are more items to retrieve.\"\n    },\n    \"first_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the first item in the list.\"\n    },\n    \"last_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the last item in the list.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-input-item-list-schema.json
tags:
- Agents
- AI
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Realtime
title: ResponseInputItemList
---
