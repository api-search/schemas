---
description: Error information.
layout: schema
name: AcrErrorInfo
properties_list:
- description: Error code.
  name: code
  type: string
- description: Error message.
  name: message
  type: string
- description: Error details.
  name: detail
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-acr-error-info-schema.json
slug: azure-container-registry-acr-error-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AcrErrorInfo\",\n  \"type\": \"object\",\n  \"description\": \"Error information.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message.\"\n    },\n    \"detail\": {\n      \"type\": \"object\",\n      \"description\": \"Error details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-acr-error-info-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: AcrErrorInfo
---
