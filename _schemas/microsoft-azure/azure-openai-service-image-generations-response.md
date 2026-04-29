---
description: Response from the image generations API.
layout: schema
name: ImageGenerationsResponse
properties_list:
- description: The Unix timestamp of when the images were created.
  name: created
  type: integer
- description: The list of generated images.
  name: data
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-image-generations-response-schema.json
slug: azure-openai-service-image-generations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageGenerationsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the image generations API.\",\n  \"properties\": {\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp of when the images were created.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of generated images.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-image-generations-response-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ImageGenerationsResponse
---
