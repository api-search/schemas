---
description: ''
layout: schema
name: ProductList
properties_list:
- description: ''
  name: products
  type: array
- description: Total product count
  name: count
  type: integer
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-product-list-schema.json
slug: archer-daniels-midland-commodity-data-api-product-list
source_filename: archer-daniels-midland-commodity-data-api-product-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"products\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"category\": {},\n          \"applications\": {},\n          \"protein\": {},\n          \"description\": {}\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total product count\",\n      \"example\": 250\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-product-list-schema.json\",\n  \"title\": \"ProductList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-product-list-schema.json
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: ProductList
---
