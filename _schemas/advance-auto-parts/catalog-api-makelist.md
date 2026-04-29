---
description: List of vehicle makes.
layout: schema
name: MakeList
properties_list:
- description: Array of vehicle makes.
  name: makes
  type: array
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-makelist-schema.json
slug: catalog-api-makelist
source_filename: catalog-api-makelist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MakeList\",\n  \"description\": \"List of vehicle makes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"makes\": {\n      \"type\": \"array\",\n      \"description\": \"Array of vehicle makes.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Make\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-makelist-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: MakeList
---
