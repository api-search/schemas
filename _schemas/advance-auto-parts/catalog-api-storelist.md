---
description: List of nearby store locations.
layout: schema
name: StoreList
properties_list:
- description: Array of store locations.
  name: stores
  type: array
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-storelist-schema.json
slug: catalog-api-storelist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StoreList\",\n  \"description\": \"List of nearby store locations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stores\": {\n      \"type\": \"array\",\n      \"description\": \"Array of store locations.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Store\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-storelist-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: StoreList
---
