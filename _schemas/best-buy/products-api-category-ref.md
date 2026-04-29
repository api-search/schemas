---
description: A reference to a product category in the hierarchy.
layout: schema
name: CategoryRef
properties_list:
- description: Category identifier.
  name: id
  type: string
- description: Category display name.
  name: name
  type: string
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/products-api-category-ref-schema.json
slug: products-api-category-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/products-api-category-ref-schema.json\",\n  \"title\": \"CategoryRef\",\n  \"description\": \"A reference to a product category in the hierarchy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Category identifier.\",\n      \"example\": \"abcat0500000\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Category display name.\",\n      \"example\": \"Computers & Tablets\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/products-api-category-ref-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: CategoryRef
---
