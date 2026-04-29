---
description: OrderResponse schema from Avalara API
layout: schema
name: OrderResponse
properties_list:
- description: ''
  name: orderId
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/business-order-response-schema.json
slug: business-order-response
source_filename: business-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-order-response-schema.json\",\n  \"title\": \"OrderResponse\",\n  \"description\": \"OrderResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Confirmed\",\n        \"Completed\",\n        \"Cancelled\"\n      ]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-order-response-schema.json
tags:
- Taxes
title: OrderResponse
---
