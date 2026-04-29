---
description: A gas supply order to Air Products
layout: schema
name: GasOrder
properties_list:
- description: Order identifier
  name: order_id
  type: string
- description: Customer account number
  name: customer_id
  type: string
- description: Product ordered
  name: product_id
  type: string
- description: Quantity ordered in specified unit
  name: quantity
  type: number
- description: Unit of measure (SCF, kg, liters)
  name: unit
  type: string
- description: Requested delivery date
  name: delivery_date
  type: string
- description: Delivery site address
  name: delivery_address
  type: string
- description: Order status
  name: status
  type: string
provider_name: Air Products and Chemicals
provider_slug: air-products-and-chemicals
schema_file: json-schema/airproducts-gas-order-schema.json
slug: airproducts-gas-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/json-schema/airproducts-gas-order-schema.json\",\n  \"title\": \"GasOrder\",\n  \"description\": \"A gas supply order to Air Products\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Order identifier\",\n      \"example\": \"ORD-2024-789012\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Customer account number\",\n      \"example\": \"CUST-10045\"\n    },\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"Product ordered\",\n      \"example\": \"N2-BULK-001\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity ordered in specified unit\",\n      \"example\": 10000.0\n    },\n    \"unit\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Unit of measure (SCF, kg, liters)\",\n      \"example\": \"SCF\"\n    },\n    \"delivery_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested delivery date\",\n      \"example\": \"2025-04-30\"\n    },\n    \"delivery_address\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery site address\",\n      \"example\": \"123 Industrial Blvd, Allentown, PA 18105\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Order status\",\n      \"example\": \"Confirmed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/json-schema/airproducts-gas-order-schema.json
tags:
- Industrial Gases
- Chemicals
- Energy
- Manufacturing
- Hydrogen
- Enterprise
title: GasOrder
---
