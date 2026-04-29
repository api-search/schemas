---
description: Common error response for all Azure Resource Manager APIs.
layout: schema
name: ErrorResponse
properties_list:
- description: The error code.
  name: code
  type: string
- description: The error message.
  name: message
  type: string
- description: The error target.
  name: target
  type: string
- description: The error details.
  name: details
  type: array
- description: The error additional info.
  name: additionalInfo
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-error-response-schema.json
slug: azure-resource-manager-error-response
source_filename: azure-resource-manager-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Common error response for all Azure Resource Manager APIs.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message.\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The error target.\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"description\": \"The error details.\"\n    },\n    \"additionalInfo\": {\n      \"type\": \"array\",\n      \"description\": \"The error additional info.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-error-response-schema.json
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
