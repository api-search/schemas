---
description: ''
layout: schema
name: ImagesResponse
properties_list:
- description: The Unix timestamp (in seconds) when the images were created.
  name: created
  type: integer
- description: The list of generated images.
  name: data
  type: array
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-images-images-response-schema.json
slug: openai-images-images-response
source_filename: openai-images-images-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImagesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp (in seconds) when the images were created.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of generated images.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-images-images-response-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: ImagesResponse
---
