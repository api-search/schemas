---
description: Specified resource.
layout: schema
name: Resource
properties_list:
- description: Resource ID.
  name: id
  type: string
- description: Resource name.
  name: name
  type: string
- description: Resource type.
  name: type
  type: string
- description: Resource location.
  name: location
  type: string
- description: Resource tags.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-resource-schema.json
slug: azure-resource-manager-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"description\": \"Specified resource.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Resource location.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-resource-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Resource
---
