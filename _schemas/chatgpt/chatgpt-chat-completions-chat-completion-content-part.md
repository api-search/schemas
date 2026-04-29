---
description: ''
layout: schema
name: ChatCompletionContentPart
properties_list:
- description: The type of the content part.
  name: type
  type: string
- description: The text content. Required when type is text.
  name: text
  type: string
- description: The image URL content. Required when type is image_url.
  name: image_url
  type: object
- description: The audio content. Required when type is input_audio.
  name: input_audio
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-chat-completion-content-part-schema.json
slug: chatgpt-chat-completions-chat-completion-content-part
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionContentPart\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content part.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content. Required when type is text.\"\n    },\n    \"image_url\": {\n      \"type\": \"object\",\n      \"description\": \"The image URL content. Required when type is image_url.\"\n    },\n    \"input_audio\": {\n      \"type\": \"object\",\n      \"description\": \"The audio content. Required when type is input_audio.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-chat-completion-content-part-schema.json
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
title: ChatCompletionContentPart
---
