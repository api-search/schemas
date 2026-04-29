---
description: ''
layout: schema
name: ResponseInputContentPart
properties_list:
- description: The type of the content part.
  name: type
  type: string
- description: The text content. Used when type is input_text.
  name: text
  type: string
- description: The URL of the image. Used when type is input_image.
  name: image_url
  type: string
- description: The detail level for image inputs.
  name: detail
  type: string
- description: The ID of the uploaded file. Used when type is input_file.
  name: file_id
  type: string
- description: The name of the file.
  name: filename
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-input-content-part-schema.json
slug: chatgpt-responses-response-input-content-part
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseInputContentPart\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content part.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content. Used when type is input_text.\"\n    },\n    \"image_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the image. Used when type is input_image.\\n\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"The detail level for image inputs.\\n\"\n    },\n    \"file_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the uploaded file. Used when type is input_file.\\n\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-input-content-part-schema.json
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
title: ResponseInputContentPart
---
