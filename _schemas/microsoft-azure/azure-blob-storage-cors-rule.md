---
description: CORS rule for the Blob service.
layout: schema
name: CorsRule
properties_list:
- description: Comma-separated list of origin domains that are allowed via CORS.
  name: AllowedOrigins
  type: string
- description: Comma-separated list of HTTP methods that are allowed. Options are DELETE, GET, HEAD, MERGE, POST, OPTIONS, PUT.
  name: AllowedMethods
  type: string
- description: Comma-separated list of headers allowed to be part of the cross-origin request.
  name: AllowedHeaders
  type: string
- description: Comma-separated list of response headers to expose to CORS clients.
  name: ExposedHeaders
  type: string
- description: The maximum amount of time in seconds that a browser should cache the preflight OPTIONS request.
  name: MaxAgeInSeconds
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-cors-rule-schema.json
slug: azure-blob-storage-cors-rule
source_filename: azure-blob-storage-cors-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CorsRule\",\n  \"type\": \"object\",\n  \"description\": \"CORS rule for the Blob service.\",\n  \"properties\": {\n    \"AllowedOrigins\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of origin domains that are allowed via CORS.\"\n    },\n    \"AllowedMethods\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of HTTP methods that are allowed. Options are DELETE, GET, HEAD, MERGE, POST, OPTIONS, PUT.\"\n    },\n    \"AllowedHeaders\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of headers allowed to be part of the cross-origin request.\"\n    },\n    \"ExposedHeaders\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of response headers to expose to CORS clients.\"\n    },\n    \"MaxAgeInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum\
  \ amount of time in seconds that a browser should cache the preflight OPTIONS request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-cors-rule-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CorsRule
---
