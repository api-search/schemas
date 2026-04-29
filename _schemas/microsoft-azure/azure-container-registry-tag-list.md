---
description: Tag list result.
layout: schema
name: TagList
properties_list:
- description: Registry name.
  name: registry
  type: string
- description: Image name.
  name: imageName
  type: string
- description: List of tag attributes.
  name: tags
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-tag-list-schema.json
slug: azure-container-registry-tag-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagList\",\n  \"type\": \"object\",\n  \"description\": \"Tag list result.\",\n  \"properties\": {\n    \"registry\": {\n      \"type\": \"string\",\n      \"description\": \"Registry name.\"\n    },\n    \"imageName\": {\n      \"type\": \"string\",\n      \"description\": \"Image name.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of tag attributes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-tag-list-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: TagList
---
