---
description: ''
layout: schema
name: ContentPart
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
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-chat-completions-content-part-schema.json
slug: openai-chat-completions-content-part
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentPart\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content part.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content. Required when type is text.\"\n    },\n    \"image_url\": {\n      \"type\": \"object\",\n      \"description\": \"The image URL content. Required when type is image_url.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-chat-completions-content-part-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: ContentPart
---
