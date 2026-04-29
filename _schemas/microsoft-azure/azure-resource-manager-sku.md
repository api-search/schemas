---
description: SKU for the resource.
layout: schema
name: Sku
properties_list:
- description: The SKU name.
  name: name
  type: string
- description: The SKU tier.
  name: tier
  type: string
- description: The SKU size.
  name: size
  type: string
- description: The SKU family.
  name: family
  type: string
- description: The SKU model.
  name: model
  type: string
- description: The SKU capacity.
  name: capacity
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-sku-schema.json
slug: azure-resource-manager-sku
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Sku\",\n  \"type\": \"object\",\n  \"description\": \"SKU for the resource.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The SKU name.\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"The SKU tier.\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"The SKU size.\"\n    },\n    \"family\": {\n      \"type\": \"string\",\n      \"description\": \"The SKU family.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The SKU model.\"\n    },\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The SKU capacity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-sku-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Sku
---
