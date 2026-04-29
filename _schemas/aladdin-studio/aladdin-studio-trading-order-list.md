---
description: Paginated list of trading orders
layout: schema
name: OrderList
properties_list:
- description: ''
  name: orders
  type: array
- description: Total number of orders
  name: totalCount
  type: integer
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-trading-order-list-schema.json
slug: aladdin-studio-trading-order-list
source_filename: aladdin-studio-trading-order-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-trading-order-list-schema.json\",\n  \"title\": \"OrderList\",\n  \"description\": \"Paginated list of trading orders\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Order\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of orders\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-trading-order-list-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: OrderList
---
