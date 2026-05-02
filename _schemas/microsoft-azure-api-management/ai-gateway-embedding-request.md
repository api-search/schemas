---
description: ''
layout: schema
name: EmbeddingRequest
properties_list:
- description: ''
  name: input
  type: string
- description: ''
  name: model
  type: string
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-embedding-request-schema.json
slug: ai-gateway-embedding-request
source_filename: ai-gateway-embedding-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddingRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"string\",\n      \"example\": \"Azure API Management provides a unified gateway for APIs.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"example\": \"text-embedding-ada-002\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-embedding-request-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: EmbeddingRequest
---
