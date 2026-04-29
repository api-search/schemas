---
description: Station search result
layout: schema
name: StationSearchResult
properties_list:
- description: ''
  name: status
  type: string
- description: List of matching stations
  name: data
  type: array
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-station-search-result-schema.json
slug: aqicn-station-search-result
source_filename: aqicn-station-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-station-search-result-schema.json\",\n  \"title\": \"StationSearchResult\",\n  \"description\": \"Station search result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"ok\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of matching stations\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"integer\",\n            \"description\": \"Station unique ID\",\n            \"example\": 8502\n          },\n          \"aqi\": {\n            \"type\": \"string\",\n            \"description\": \"Current AQI value or \\\"N/A\\\"\",\n            \"example\": \"45\"\n          },\n          \"station\": {\n       \
  \     \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Station name\",\n                \"example\": \"Beijing, China\"\n              },\n              \"geo\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"number\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-station-search-result-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: StationSearchResult
---
