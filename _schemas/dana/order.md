---
description: An aftermarket order placed through the Dana Aftermarket API.
layout: schema
name: Order
properties_list:
- description: ''
  name: orderId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: items
  type: array
- description: ''
  name: shippingAddress
  type: object
- description: ''
  name: trackingNumber
  type: string
provider_name: Dana
provider_slug: dana
schema_file: json-schema/order.json
slug: order
source_filename: order.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/json-schema/order.json\",\n  \"title\": \"Order\",\n  \"description\": \"An aftermarket order placed through the Dana Aftermarket API.\",\n  \"type\": \"object\",\n  \"required\": [\"items\"],\n  \"properties\": {\n    \"orderId\": {\"type\": \"string\"},\n    \"status\": {\"type\": \"string\"},\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"partNumber\", \"quantity\"],\n        \"properties\": {\n          \"partNumber\": {\"type\": \"string\"},\n          \"quantity\": {\"type\": \"integer\", \"minimum\": 1}\n        }\n      }\n    },\n    \"shippingAddress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\"type\": \"string\"},\n        \"street\": {\"type\": \"string\"},\n        \"city\": {\"type\": \"string\"},\n \
  \       \"region\": {\"type\": \"string\"},\n        \"postalCode\": {\"type\": \"string\"},\n        \"country\": {\"type\": \"string\"}\n      }\n    },\n    \"trackingNumber\": {\"type\": \"string\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/json-schema/order.json
tags:
- Aftermarket
- Auto Parts
- Drivetrain
- eCommerce
- Supply Chain
title: Order
---
