---
description: Plan for the resource.
layout: schema
name: Plan
properties_list:
- description: The plan ID.
  name: name
  type: string
- description: The publisher ID.
  name: publisher
  type: string
- description: The offer ID.
  name: product
  type: string
- description: The promotion code.
  name: promotionCode
  type: string
- description: The plan's version.
  name: version
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-plan-schema.json
slug: azure-resource-manager-plan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Plan\",\n  \"type\": \"object\",\n  \"description\": \"Plan for the resource.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The plan ID.\"\n    },\n    \"publisher\": {\n      \"type\": \"string\",\n      \"description\": \"The publisher ID.\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"The offer ID.\"\n    },\n    \"promotionCode\": {\n      \"type\": \"string\",\n      \"description\": \"The promotion code.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The plan's version.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-plan-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Plan
---
