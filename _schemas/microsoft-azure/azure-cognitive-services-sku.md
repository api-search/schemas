---
description: The resource model definition representing SKU.
layout: schema
name: Sku
properties_list:
- description: The name of the SKU. Examples include F0 (free), S0, S1, S2, etc.
  name: name
  type: string
- description: The pricing tier of the SKU.
  name: tier
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-sku-schema.json
slug: azure-cognitive-services-sku
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Sku\",\n  \"type\": \"object\",\n  \"description\": \"The resource model definition representing SKU.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the SKU. Examples include F0 (free), S0, S1, S2, etc.\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"The pricing tier of the SKU.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-sku-schema.json
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
