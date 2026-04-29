---
description: Data source attribution
layout: schema
name: Attribution
properties_list:
- description: Attribution URL
  name: url
  type: string
- description: Data source name
  name: name
  type: string
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-attribution-schema.json
slug: aqicn-attribution
source_filename: aqicn-attribution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-attribution-schema.json\",\n  \"title\": \"Attribution\",\n  \"description\": \"Data source attribution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Attribution URL\",\n      \"example\": \"https://www.epa.gov/airnow\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\",\n      \"example\": \"US EPA AirNow\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-attribution-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: Attribution
---
