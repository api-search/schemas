---
description: Request body for creating image generations.
layout: schema
name: CreateImageRequest
properties_list:
- description: A text description of the desired image(s).
  name: prompt
  type: string
- description: The number of images to generate.
  name: n
  type: integer
- description: The size of the generated images.
  name: size
  type: string
- description: The quality of the image that will be generated.
  name: quality
  type: string
- description: The style of the generated images.
  name: style
  type: string
- description: The format in which the generated images are returned.
  name: response_format
  type: string
- description: A unique identifier representing your end-user.
  name: user
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-image-request-schema.json
slug: azure-openai-service-create-image-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateImageRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating image generations.\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"A text description of the desired image(s).\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of images to generate.\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"The size of the generated images.\"\n    },\n    \"quality\": {\n      \"type\": \"string\",\n      \"description\": \"The quality of the image that will be generated.\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"The style of the generated images.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\",\n      \"description\": \"The format in which the generated images are returned.\"\n    },\n    \"\
  user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-image-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateImageRequest
---
