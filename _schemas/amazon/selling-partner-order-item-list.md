---
description: OrderItemList schema from Amazon Selling Partner API
layout: schema
name: OrderItemList
properties_list:
- description: ''
  name: payload
  type: object
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-order-item-list-schema.json
slug: selling-partner-order-item-list
source_filename: selling-partner-order-item-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OrderItems\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/OrderItem\"\n          }\n        },\n        \"NextToken\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrderItemList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-order-item-list-schema.json\",\n  \"description\": \"OrderItemList schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-order-item-list-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: OrderItemList
---
