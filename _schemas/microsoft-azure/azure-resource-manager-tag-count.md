---
description: Tag count.
layout: schema
name: TagCount
properties_list:
- description: Type of count.
  name: type
  type: string
- description: Value of count.
  name: value
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-tag-count-schema.json
slug: azure-resource-manager-tag-count
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagCount\",\n  \"type\": \"object\",\n  \"description\": \"Tag count.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of count.\"\n    },\n    \"value\": {\n      \"type\": \"integer\",\n      \"description\": \"Value of count.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-tag-count-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: TagCount
---
