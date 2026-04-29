---
description: Represents an order for products and services.
layout: schema
name: Order
properties_list:
- description: Unique ID for this order.
  name: id
  type: string
- description: The ID of the seller location that this order is associated with.
  name: location_id
  type: string
- description: Current state of the order.
  name: state
  type: string
- description: Version number for optimistic concurrency control.
  name: version
  type: integer
- description: Total amount for the order.
  name: total_money
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Block
provider_slug: block
schema_file: json-schema/block-order-schema.json
slug: block-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/block/main/json-schema/block-order-schema.json\",\n  \"title\": \"Order\",\n  \"description\": \"Represents an order for products and services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for this order.\",\n      \"example\": \"CAISENgvlJ6jLWAzERDzjyHVybY\"\n    },\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the seller location that this order is associated with.\",\n      \"example\": \"L1234567890\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the order.\",\n      \"enum\": [\"OPEN\", \"COMPLETED\", \"CANCELED\", \"DRAFT\"],\n      \"example\": \"OPEN\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number for optimistic\
  \ concurrency control.\",\n      \"example\": 1\n    },\n    \"total_money\": {\n      \"type\": \"object\",\n      \"description\": \"Total amount for the order.\",\n      \"properties\": {\n        \"amount\": { \"type\": \"integer\", \"example\": 3000 },\n        \"currency\": { \"type\": \"string\", \"example\": \"USD\" }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:05:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:05:00Z\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/json-schema/block-order-schema.json
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: Order
---
