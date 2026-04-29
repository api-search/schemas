---
description: Tag information.
layout: schema
name: TagValue
properties_list:
- description: The tag value ID.
  name: id
  type: string
- description: The tag value.
  name: tagValue
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-tag-value-schema.json
slug: azure-resource-manager-tag-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagValue\",\n  \"type\": \"object\",\n  \"description\": \"Tag information.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value ID.\"\n    },\n    \"tagValue\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-tag-value-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: TagValue
---
