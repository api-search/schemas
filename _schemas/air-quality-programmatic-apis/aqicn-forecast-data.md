---
description: Multi-day air quality and weather forecast
layout: schema
name: ForecastData
properties_list:
- description: Daily forecasts by pollutant
  name: daily
  type: object
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-forecast-data-schema.json
slug: aqicn-forecast-data
source_filename: aqicn-forecast-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-forecast-data-schema.json\",\n  \"title\": \"ForecastData\",\n  \"description\": \"Multi-day air quality and weather forecast\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"daily\": {\n      \"type\": \"object\",\n      \"description\": \"Daily forecasts by pollutant\",\n      \"properties\": {\n        \"pm25\": {\n          \"type\": \"array\",\n          \"description\": \"PM2.5 daily forecast values\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ForecastDay\"\n          }\n        },\n        \"pm10\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ForecastDay\"\n          }\n        },\n        \"o3\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ForecastDay\"\
  \n          }\n        },\n        \"uvi\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ForecastDay\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-forecast-data-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: ForecastData
---
