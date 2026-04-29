---
description: The resource management error additional info.
layout: schema
name: ErrorAdditionalInfo
properties_list:
- description: The additional info type.
  name: type
  type: string
- description: The additional info.
  name: info
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-error-additional-info-schema.json
slug: azure-resource-manager-error-additional-info
source_filename: azure-resource-manager-error-additional-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorAdditionalInfo\",\n  \"type\": \"object\",\n  \"description\": \"The resource management error additional info.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The additional info type.\"\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"The additional info.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-error-additional-info-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ErrorAdditionalInfo
---
