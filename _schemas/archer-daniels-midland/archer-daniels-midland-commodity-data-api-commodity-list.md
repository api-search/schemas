---
description: ''
layout: schema
name: CommodityList
properties_list:
- description: ''
  name: commodities
  type: array
- description: Total commodity count
  name: count
  type: integer
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-commodity-list-schema.json
slug: archer-daniels-midland-commodity-data-api-commodity-list
source_filename: archer-daniels-midland-commodity-data-api-commodity-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"commodities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"type\": {},\n          \"currentPrice\": {},\n          \"currency\": {},\n          \"unit\": {},\n          \"priceDate\": {}\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total commodity count\",\n      \"example\": 15\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-commodity-list-schema.json\",\n  \"title\": \"CommodityList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-commodity-list-schema.json
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: CommodityList
---
