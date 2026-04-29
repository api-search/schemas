---
description: List of orders
layout: schema
name: OrderList
properties_list:
- description: Array of order records
  name: orders
  type: array
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-order-list-schema.json
slug: 3m-partner-supplier-api-order-list
source_filename: 3m-partner-supplier-api-order-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-order-list-schema.json\",\n  \"title\": \"OrderList\",\n  \"description\": \"List of orders\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orders\": {\n      \"type\": \"array\",\n      \"description\": \"Array of order records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Order\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-order-list-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: OrderList
---
