---
description: List of 3M products
layout: schema
name: ProductList
properties_list:
- description: Array of product records
  name: products
  type: array
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-product-list-schema.json
slug: 3m-partner-supplier-api-product-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-product-list-schema.json\",\n  \"title\": \"ProductList\",\n  \"description\": \"List of 3M products\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"Array of product records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Product\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-product-list-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: ProductList
---
