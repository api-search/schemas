---
description: ''
layout: schema
name: PendingProductOrder
properties_list:
- description: Type of product order, e.g. 'Add' or 'Remove'.
  name: type
  type: string
- description: Status of the pending product order.
  name: status
  type: string
- description: Date and time when product was ordered.
  name: requested
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-pending-product-order-schema.json
slug: factset-procure-to-pay-scim-pending-product-order
source_filename: factset-procure-to-pay-scim-pending-product-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PendingProductOrder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of product order, e.g. 'Add' or 'Remove'.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the pending product order.\"\n    },\n    \"requested\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when product was ordered.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-pending-product-order-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PendingProductOrder
---
