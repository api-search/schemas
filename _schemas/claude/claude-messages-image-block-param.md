---
description: An image content block. Supports base64-encoded or URL-referenced images.
layout: schema
name: ImageBlockParam
properties_list:
- description: ''
  name: type
  type: string
- description: The source of the image.
  name: source
  type: object
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-image-block-param-schema.json
slug: claude-messages-image-block-param
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageBlockParam\",\n  \"type\": \"object\",\n  \"description\": \"An image content block. Supports base64-encoded or URL-referenced images.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The source of the image.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-image-block-param-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ImageBlockParam
---
