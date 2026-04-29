---
description: ''
layout: schema
name: CreateImageVariationRequest
properties_list:
- description: The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square.
  name: image
  type: string
- description: The model to use for image variation. Only DALL-E 2 is supported.
  name: model
  type: string
- description: The number of images to generate.
  name: n
  type: integer
- description: The format in which the generated images are returned.
  name: response_format
  type: string
- description: The size of the generated images.
  name: size
  type: string
- description: A unique identifier representing your end-user.
  name: user
  type: string
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-images-create-image-variation-request-schema.json
slug: openai-images-create-image-variation-request
source_filename: openai-images-create-image-variation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateImageVariationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model to use for image variation. Only DALL-E 2 is supported.\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of images to generate.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\",\n      \"description\": \"The format in which the generated images are returned.\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"The size of the generated images.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-images-create-image-variation-request-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: CreateImageVariationRequest
---
