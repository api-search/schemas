---
description: ''
layout: schema
name: LocationList
properties_list:
- description: ''
  name: locations
  type: array
- description: Total location count
  name: count
  type: integer
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-location-list-schema.json
slug: archer-daniels-midland-commodity-data-api-location-list
source_filename: archer-daniels-midland-commodity-data-api-location-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"locations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"type\": {},\n          \"country\": {},\n          \"state\": {},\n          \"city\": {},\n          \"latitude\": {},\n          \"longitude\": {}\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total location count\",\n      \"example\": 200\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-location-list-schema.json\",\n  \"title\": \"LocationList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-location-list-schema.json
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: LocationList
---
