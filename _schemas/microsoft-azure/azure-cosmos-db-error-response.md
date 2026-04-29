---
description: Error response from Cosmos DB.
layout: schema
name: ErrorResponse
properties_list:
- description: The error code.
  name: code
  type: string
- description: The error message.
  name: message
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-error-response-schema.json
slug: azure-cosmos-db-error-response
source_filename: azure-cosmos-db-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error response from Cosmos DB.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-error-response-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ErrorResponse
---
