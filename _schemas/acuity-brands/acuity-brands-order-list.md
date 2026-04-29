---
description: Paginated list of orders
layout: schema
name: OrderList
properties_list:
- description: ''
  name: orders
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: cursor
  type: string
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-order-list-schema.json
slug: acuity-brands-order-list
source_filename: acuity-brands-order-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-order-list-schema.json\",\n  \"title\": \"OrderList\",\n  \"description\": \"Paginated list of orders\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Order\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 200\n    },\n    \"cursor\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-order-list-schema.json
tags: []
title: OrderList
---
