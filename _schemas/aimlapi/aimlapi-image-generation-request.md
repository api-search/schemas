---
description: Request body for generating an image via AIMLAPI
layout: schema
name: ImageGenerationRequest
properties_list:
- description: Image generation model ID
  name: model
  type: string
- description: Text description of desired image
  name: prompt
  type: string
- description: Number of images to generate
  name: n
  type: integer
- description: Image dimensions
  name: size
  type: string
- description: Image quality (standard, hd)
  name: quality
  type: string
- description: Image style (vivid, natural)
  name: style
  type: string
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-image-generation-request-schema.json
slug: aimlapi-image-generation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-image-generation-request-schema.json\",\n  \"title\": \"ImageGenerationRequest\",\n  \"description\": \"Request body for generating an image via AIMLAPI\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Image generation model ID\",\n      \"example\": \"dall-e-3\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text description of desired image\",\n      \"example\": \"A futuristic cityscape at sunset\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of images to generate\",\n      \"example\": 1\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Image dimensions\",\n      \"example\": \"1024x1024\"\n    },\n    \"quality\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"Image quality (standard, hd)\",\n      \"example\": \"standard\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Image style (vivid, natural)\",\n      \"example\": \"vivid\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-image-generation-request-schema.json
tags:
- Artificial Intelligence
- Machine Learning
- AI Models
- LLM
- Image Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
title: ImageGenerationRequest
---
