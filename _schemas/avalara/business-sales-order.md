---
description: SalesOrder schema from Avalara API
layout: schema
name: SalesOrder
properties_list:
- description: ''
  name: accountId
  type: string
- description: ''
  name: products
  type: array
- description: ''
  name: campaignId
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/business-sales-order-schema.json
slug: business-sales-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-sales-order-schema.json\",\n  \"title\": \"SalesOrder\",\n  \"description\": \"SalesOrder schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"accountId\",\n    \"products\"\n  ],\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"productCode\": {\n            \"type\": \"string\"\n          },\n          \"quantity\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"campaignId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-sales-order-schema.json
tags:
- Taxes
title: SalesOrder
---
