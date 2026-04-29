---
description: Tag details.
layout: schema
name: TagDetails
properties_list:
- description: The tag name ID.
  name: id
  type: string
- description: The tag name.
  name: tagName
  type: string
- description: The list of tag values.
  name: values
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-tag-details-schema.json
slug: azure-resource-manager-tag-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagDetails\",\n  \"type\": \"object\",\n  \"description\": \"Tag details.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The tag name ID.\"\n    },\n    \"tagName\": {\n      \"type\": \"string\",\n      \"description\": \"The tag name.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tag values.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-tag-details-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: TagDetails
---
