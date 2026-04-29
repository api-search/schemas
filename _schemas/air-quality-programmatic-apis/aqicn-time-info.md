---
description: Timestamp information for the reading
layout: schema
name: TimeInfo
properties_list:
- description: ISO 8601 timestamp of measurement
  name: s
  type: string
- description: Station timezone
  name: tz
  type: string
- description: Unix timestamp
  name: v
  type: integer
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-time-info-schema.json
slug: aqicn-time-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-time-info-schema.json\",\n  \"title\": \"TimeInfo\",\n  \"description\": \"Timestamp information for the reading\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp of measurement\",\n      \"example\": \"2025-04-19 10:00:00\"\n    },\n    \"tz\": {\n      \"type\": \"string\",\n      \"description\": \"Station timezone\",\n      \"example\": \"+08:00\"\n    },\n    \"v\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp\",\n      \"example\": 1745056800\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-time-info-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: TimeInfo
---
