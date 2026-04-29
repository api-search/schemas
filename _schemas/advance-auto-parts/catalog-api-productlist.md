---
description: List of products matching search criteria.
layout: schema
name: ProductList
properties_list:
- description: Array of products.
  name: products
  type: array
- description: Total number of matching products.
  name: total
  type: integer
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-productlist-schema.json
slug: catalog-api-productlist
source_filename: catalog-api-productlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProductList\",\n  \"description\": \"List of products matching search criteria.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"Array of products.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Product\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching products.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-productlist-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: ProductList
---
