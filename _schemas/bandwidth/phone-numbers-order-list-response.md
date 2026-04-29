---
description: Response containing a list of orders
layout: schema
name: OrderListResponse
properties_list:
- description: Total number of orders
  name: totalCount
  type: integer
- description: ''
  name: orders
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-order-list-response-schema.json
slug: phone-numbers-order-list-response
source_filename: phone-numbers-order-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-order-list-response-schema.json\",\n  \"title\": \"OrderListResponse\",\n  \"description\": \"Response containing a list of orders\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of orders\"\n    },\n    \"orders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OrderResponse\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-order-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: OrderListResponse
---
