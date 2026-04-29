---
description: List of Alaska Airlines served airports
layout: schema
name: AirportList
properties_list:
- description: ''
  name: airports
  type: array
- description: Total airport count
  name: totalCount
  type: integer
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-schedules-airport-list-schema.json
slug: alaska-air-flight-schedules-airport-list
source_filename: alaska-air-flight-schedules-airport-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-airport-list-schema.json\",\n  \"title\": \"AirportList\",\n  \"description\": \"List of Alaska Airlines served airports\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"airports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AirportInfo\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total airport count\",\n      \"example\": 115\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-airport-list-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: AirportList
---
