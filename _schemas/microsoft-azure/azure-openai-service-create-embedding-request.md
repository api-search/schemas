---
description: Request body for creating embeddings.
layout: schema
name: CreateEmbeddingRequest
properties_list:
- description: Input text to embed, encoded as a string or array of strings.
  name: input
  type: string
- description: A unique identifier representing your end-user.
  name: user
  type: string
- description: The input type for the embedding request.
  name: input_type
  type: string
- description: The format to return the embeddings in.
  name: encoding_format
  type: string
- description: The number of dimensions the resulting output embeddings should have.
  name: dimensions
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-embedding-request-schema.json
slug: azure-openai-service-create-embedding-request
source_filename: azure-openai-service-create-embedding-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEmbeddingRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating embeddings.\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"Input text to embed, encoded as a string or array of strings.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user.\"\n    },\n    \"input_type\": {\n      \"type\": \"string\",\n      \"description\": \"The input type for the embedding request.\"\n    },\n    \"encoding_format\": {\n      \"type\": \"string\",\n      \"description\": \"The format to return the embeddings in.\"\n    },\n    \"dimensions\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of dimensions the resulting output embeddings should have.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-embedding-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateEmbeddingRequest
---
