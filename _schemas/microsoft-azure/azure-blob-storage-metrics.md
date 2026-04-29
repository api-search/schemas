---
description: Storage analytics metrics settings.
layout: schema
name: Metrics
properties_list:
- description: ''
  name: Version
  type: string
- description: ''
  name: Enabled
  type: boolean
- description: ''
  name: IncludeAPIs
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-metrics-schema.json
slug: azure-blob-storage-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metrics\",\n  \"type\": \"object\",\n  \"description\": \"Storage analytics metrics settings.\",\n  \"properties\": {\n    \"Version\": {\n      \"type\": \"string\"\n    },\n    \"Enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"IncludeAPIs\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-metrics-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Metrics
---
