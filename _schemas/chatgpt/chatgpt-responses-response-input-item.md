---
description: ''
layout: schema
name: ResponseInputItem
properties_list:
- description: The role of the input item.
  name: role
  type: string
- description: The content of the input item. Can be a string or an array of content parts for multimodal input.
  name: content
  type: string
- description: The type of the input item. Typically message for conversation messages, or specialized types like function_call_output.
  name: type
  type: string
- description: The unique ID of the input item. Used for item_reference type.
  name: id
  type: string
- description: The ID of the function call this output corresponds to. Required for function_call_output type.
  name: call_id
  type: string
- description: The output of the function call. Required for function_call_output type.
  name: output
  type: string
- description: The status of the input item.
  name: status
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-input-item-schema.json
slug: chatgpt-responses-response-input-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseInputItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the input item.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the input item. Can be a string or an array\\nof content parts for multimodal input.\\n\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the input item. Typically message for\\nconversation messages, or specialized types like\\nfunction_call_output.\\n\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the input item. Used for item_reference type.\\n\"\n    },\n    \"call_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the function call this output corresponds to.\\nRequired for function_call_output type.\\n\"\n   \
  \ },\n    \"output\": {\n      \"type\": \"string\",\n      \"description\": \"The output of the function call. Required for\\nfunction_call_output type.\\n\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the input item.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-input-item-schema.json
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
title: ResponseInputItem
---
