---
description: Single-day forecast value
layout: schema
name: ForecastDay
properties_list:
- description: Average AQI for the day
  name: avg
  type: integer
- description: Date string
  name: day
  type: string
- description: Maximum AQI for the day
  name: max
  type: integer
- description: Minimum AQI for the day
  name: min
  type: integer
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-forecast-day-schema.json
slug: aqicn-forecast-day
source_filename: aqicn-forecast-day-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-forecast-day-schema.json\",\n  \"title\": \"ForecastDay\",\n  \"description\": \"Single-day forecast value\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"avg\": {\n      \"type\": \"integer\",\n      \"description\": \"Average AQI for the day\",\n      \"example\": 52\n    },\n    \"day\": {\n      \"type\": \"string\",\n      \"description\": \"Date string\",\n      \"example\": \"2025-04-20\"\n    },\n    \"max\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum AQI for the day\",\n      \"example\": 78\n    },\n    \"min\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum AQI for the day\",\n      \"example\": 31\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-forecast-day-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: ForecastDay
---
