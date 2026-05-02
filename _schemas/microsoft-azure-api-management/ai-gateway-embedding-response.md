---
description: ''
layout: schema
name: EmbeddingResponse
properties_list:
- description: ''
  name: object
  type: string
- description: ''
  name: data
  type: array
- description: ''
  name: model
  type: string
- description: ''
  name: usage
  type: object
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-embedding-response-schema.json
slug: ai-gateway-embedding-response
source_filename: ai-gateway-embedding-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddingResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"object\": {\n            \"type\": \"string\",\n            \"example\": \"embedding\"\n          },\n          \"index\": {\n            \"type\": \"integer\",\n            \"example\": 0\n          },\n          \"embedding\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"number\"\n            }\n          }\n        }\n      }\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"example\": \"text-embedding-ada-002\"\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prompt_tokens\": {\n          \"type\": \"integer\"\
  ,\n          \"example\": 12\n        },\n        \"total_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 12\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-embedding-response-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: EmbeddingResponse
---
