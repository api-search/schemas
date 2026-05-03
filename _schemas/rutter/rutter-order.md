---
description: A commerce order from a connected platform via the Rutter Unified API
layout: schema
name: Rutter Order
properties_list:
- description: Unique identifier for the order
  name: id
  type: string
- description: The ID of the customer who placed the order
  name: customer_id
  type: string
- description: Current order status
  name: status
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Total order price
  name: total_price
  type: number
- description: ''
  name: line_items
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Rutter
provider_slug: rutter
schema_file: json-schema/rutter-order-schema.json
slug: rutter-order
source_filename: rutter-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rutter/json-schema/rutter-order-schema.json\",\n  \"title\": \"Rutter Order\",\n  \"description\": \"A commerce order from a connected platform via the Rutter Unified API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the order\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the customer who placed the order\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"processing\", \"fulfilled\", \"cancelled\"],\n      \"description\": \"Current order status\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"total_price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total order price\"\
  \n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderLineItem\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"status\"],\n  \"$defs\": {\n    \"OrderLineItem\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"product_id\": {\n          \"type\": \"string\"\n        },\n        \"variant_id\": {\n          \"type\": \"string\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\"\n        },\n        \"unit_price\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rutter/refs/heads/main/json-schema/rutter-order-schema.json
tags:
- Accounting
- B2B
- Commerce
- Financial Data
- Payments
- Unified API
title: Rutter Order
---
