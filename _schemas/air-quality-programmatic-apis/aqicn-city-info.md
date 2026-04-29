---
description: City and location information for the station
layout: schema
name: CityInfo
properties_list:
- description: City and station name
  name: name
  type: string
- description: Station URL on AQICN
  name: url
  type: string
- description: Geographic coordinates [latitude, longitude]
  name: geo
  type: array
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-city-info-schema.json
slug: aqicn-city-info
source_filename: aqicn-city-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-city-info-schema.json\",\n  \"title\": \"CityInfo\",\n  \"description\": \"City and location information for the station\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"City and station name\",\n      \"example\": \"Beijing, China\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Station URL on AQICN\",\n      \"example\": \"https://aqicn.org/city/beijing/\"\n    },\n    \"geo\": {\n      \"type\": \"array\",\n      \"description\": \"Geographic coordinates [latitude, longitude]\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"example\": [\n        39.9042,\n        116.4074\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-city-info-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: CityInfo
---
