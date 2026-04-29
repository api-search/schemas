---
description: Tag attribute details.
layout: schema
name: TagAttributesBase
properties_list:
- description: Tag name.
  name: name
  type: string
- description: Tag digest.
  name: digest
  type: string
- description: ''
  name: createdTime
  type: string
- description: ''
  name: lastUpdateTime
  type: string
- description: Whether the tag is signed.
  name: signed
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-tag-attributes-base-schema.json
slug: azure-container-registry-tag-attributes-base
source_filename: azure-container-registry-tag-attributes-base-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagAttributesBase\",\n  \"type\": \"object\",\n  \"description\": \"Tag attribute details.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tag name.\"\n    },\n    \"digest\": {\n      \"type\": \"string\",\n      \"description\": \"Tag digest.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"string\"\n    },\n    \"signed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the tag is signed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-tag-attributes-base-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: TagAttributesBase
---
