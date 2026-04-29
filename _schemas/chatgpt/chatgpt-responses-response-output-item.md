---
description: ''
layout: schema
name: ResponseOutputItem
properties_list:
- description: The type of the output item.
  name: type
  type: string
- description: The unique ID of the output item.
  name: id
  type: string
- description: The role of the output item.
  name: role
  type: string
- description: The status of the output item.
  name: status
  type: string
- description: The content of the output message. Present when type is message.
  name: content
  type: array
- description: The name of the function being called. Present when type is function_call.
  name: name
  type: string
- description: The unique ID of the function call. Present when type is function_call.
  name: call_id
  type: string
- description: The arguments to the function call in JSON format. Present when type is function_call.
  name: arguments
  type: string
- description: A summary of the reasoning performed by the model. Present when type is reasoning.
  name: summary
  type: array
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-output-item-schema.json
slug: chatgpt-responses-response-output-item
source_filename: chatgpt-responses-response-output-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseOutputItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the output item.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the output item.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the output item.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the output item.\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The content of the output message. Present when type\\nis message.\\n\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function being called. Present when type\\nis function_call.\\n\"\n    },\n    \"call_id\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The unique ID of the function call. Present when type is\\nfunction_call.\\n\"\n    },\n    \"arguments\": {\n      \"type\": \"string\",\n      \"description\": \"The arguments to the function call in JSON format. Present\\nwhen type is function_call.\\n\"\n    },\n    \"summary\": {\n      \"type\": \"array\",\n      \"description\": \"A summary of the reasoning performed by the model. Present\\nwhen type is reasoning.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-output-item-schema.json
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
title: ResponseOutputItem
---
