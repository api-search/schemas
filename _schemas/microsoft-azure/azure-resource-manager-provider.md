---
description: Resource provider information.
layout: schema
name: Provider
properties_list:
- description: The provider ID.
  name: id
  type: string
- description: The namespace of the resource provider.
  name: namespace
  type: string
- description: The registration state of the resource provider.
  name: registrationState
  type: string
- description: The registration policy of the resource provider.
  name: registrationPolicy
  type: string
- description: The collection of provider resource types.
  name: resourceTypes
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-provider-schema.json
slug: azure-resource-manager-provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Provider\",\n  \"type\": \"object\",\n  \"description\": \"Resource provider information.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The provider ID.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the resource provider.\"\n    },\n    \"registrationState\": {\n      \"type\": \"string\",\n      \"description\": \"The registration state of the resource provider.\"\n    },\n    \"registrationPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The registration policy of the resource provider.\"\n    },\n    \"resourceTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of provider resource types.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-provider-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Provider
---
