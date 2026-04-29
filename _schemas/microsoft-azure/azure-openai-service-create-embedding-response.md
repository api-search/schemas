---
description: Response from the embeddings API.
layout: schema
name: CreateEmbeddingResponse
properties_list:
- description: The object type.
  name: object
  type: string
- description: The list of embeddings generated.
  name: data
  type: array
- description: The model used to generate the embeddings.
  name: model
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-embedding-response-schema.json
slug: azure-openai-service-create-embedding-response
source_filename: azure-openai-service-create-embedding-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEmbeddingResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the embeddings API.\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of embeddings generated.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used to generate the embeddings.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-embedding-response-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateEmbeddingResponse
---
