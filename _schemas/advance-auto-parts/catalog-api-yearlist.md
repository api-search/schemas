---
description: List of available vehicle model years.
layout: schema
name: YearList
properties_list:
- description: Array of model years.
  name: years
  type: array
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-yearlist-schema.json
slug: catalog-api-yearlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"YearList\",\n  \"description\": \"List of available vehicle model years.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"years\": {\n      \"type\": \"array\",\n      \"description\": \"Array of model years.\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-yearlist-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: YearList
---
