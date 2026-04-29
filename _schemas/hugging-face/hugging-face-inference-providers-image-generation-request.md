---
description: ''
layout: schema
name: ImageGenerationRequest
properties_list:
- description: Image generation model ID
  name: model
  type: string
- description: Text prompt describing the image to generate
  name: prompt
  type: string
- description: Number of images to generate
  name: n
  type: integer
- description: Image dimensions
  name: size
  type: string
- description: ''
  name: response_format
  type: string
- description: Negative prompt to guide generation
  name: negative_prompt
  type: string
- description: Number of diffusion steps
  name: num_inference_steps
  type: integer
- description: Classifier-free guidance scale
  name: guidance_scale
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-providers-image-generation-request-schema.json
slug: hugging-face-inference-providers-image-generation-request
source_filename: hugging-face-inference-providers-image-generation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageGenerationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Image generation model ID\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text prompt describing the image to generate\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of images to generate\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Image dimensions\"\n    },\n    \"response_format\": {\n      \"type\": \"string\"\n    },\n    \"negative_prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Negative prompt to guide generation\"\n    },\n    \"num_inference_steps\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of diffusion steps\"\n    },\n    \"guidance_scale\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Classifier-free guidance scale\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-providers-image-generation-request-schema.json
tags: []
title: ImageGenerationRequest
---
