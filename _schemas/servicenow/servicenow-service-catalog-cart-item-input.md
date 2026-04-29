---
description: Input for adding a catalog item to the cart or ordering directly.
layout: schema
name: CartItemInput
properties_list:
- description: The quantity of items to order.
  name: sysparm_quantity
  type: integer
- description: Name-value pairs for the catalog item variables. Keys are variable names and values are the user-provided entries.
  name: variables
  type: object
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-cart-item-input-schema.json
slug: servicenow-service-catalog-cart-item-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for adding a catalog item to the cart or ordering directly.\",\n  \"properties\": {\n    \"sysparm_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"The quantity of items to order.\",\n      \"example\": 10\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Name-value pairs for the catalog item variables. Keys are variable names and values are the user-provided entries.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"sysparm_quantity\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CartItemInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-cart-item-input-schema.json
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
title: CartItemInput
---
