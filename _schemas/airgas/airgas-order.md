---
description: An Airgas B2B customer order for industrial gases, welding, or safety products.
layout: schema
name: Order
properties_list:
- description: Unique order number.
  name: order_number
  type: string
- description: Customer account number.
  name: account_number
  type: string
- description: Current order status.
  name: status
  type: string
- description: Date and time the order was placed.
  name: order_date
  type: string
- description: Scheduled or actual delivery date.
  name: delivery_date
  type: string
- description: Customer purchase order number.
  name: purchase_order
  type: string
- description: Delivery address for the order.
  name: delivery_address
  type: object
- description: Products included in the order.
  name: line_items
  type: array
- description: Total order amount.
  name: total_amount
  type: number
provider_name: Airgas
provider_slug: airgas
schema_file: json-schema/airgas-order-schema.json
slug: airgas-order
source_filename: airgas-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airgas/refs/heads/main/json-schema/airgas-order-schema.json\",\n  \"title\": \"Order\",\n  \"description\": \"An Airgas B2B customer order for industrial gases, welding, or safety products.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"order_number\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order number.\",\n      \"example\": \"AG-2026-00123456\"\n    },\n    \"account_number\": {\n      \"type\": \"string\",\n      \"description\": \"Customer account number.\",\n      \"example\": \"ACCT-789012\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"confirmed\", \"processing\", \"shipped\", \"delivered\", \"cancelled\"],\n      \"description\": \"Current order status.\",\n      \"example\": \"confirmed\"\n    },\n    \"order_date\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Date and time the order was placed.\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    },\n    \"delivery_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Scheduled or actual delivery date.\",\n      \"example\": \"2026-04-22\"\n    },\n    \"purchase_order\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order number.\",\n      \"example\": \"PO-20260419-001\"\n    },\n    \"delivery_address\": {\n      \"type\": \"object\",\n      \"description\": \"Delivery address for the order.\",\n      \"properties\": {\n        \"street\": {\"type\": \"string\", \"example\": \"123 Industrial Blvd\"},\n        \"city\": {\"type\": \"string\", \"example\": \"Houston\"},\n        \"state\": {\"type\": \"string\", \"example\": \"TX\"},\n        \"zip\": {\"type\": \"string\", \"example\": \"77001\"},\n        \"country\": {\"type\": \"string\", \"example\": \"US\"}\n      }\n    },\n\
  \    \"line_items\": {\n      \"type\": \"array\",\n      \"description\": \"Products included in the order.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product_number\": {\"type\": \"string\"},\n          \"quantity\": {\"type\": \"integer\"},\n          \"unit_price\": {\"type\": \"number\"}\n        }\n      }\n    },\n    \"total_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total order amount.\",\n      \"example\": 523.75\n    }\n  },\n  \"required\": [\"order_number\", \"account_number\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airgas/refs/heads/main/json-schema/airgas-order-schema.json
tags:
- Industrial Gases
- Welding
- Safety
- B2B
- Supply Chain
- Manufacturing
- Healthcare
title: Order
---
