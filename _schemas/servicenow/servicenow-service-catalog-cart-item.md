---
description: An item in the shopping cart.
layout: schema
name: CartItem
properties_list:
- description: Unique identifier for the cart item.
  name: cart_item_id
  type: string
- description: The sys_id of the catalog item.
  name: catalog_item_id
  type: string
- description: The quantity ordered.
  name: quantity
  type: integer
- description: The subtotal for this cart item.
  name: subtotal
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-cart-item-schema.json
slug: servicenow-service-catalog-cart-item
source_filename: servicenow-service-catalog-cart-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An item in the shopping cart.\",\n  \"properties\": {\n    \"cart_item_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the cart item.\",\n      \"example\": \"500123\"\n    },\n    \"catalog_item_id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the catalog item.\",\n      \"example\": \"500123\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"The quantity ordered.\",\n      \"example\": 10\n    },\n    \"subtotal\": {\n      \"type\": \"string\",\n      \"description\": \"The subtotal for this cart item.\",\n      \"example\": 42\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CartItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-cart-item-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: CartItem
---
