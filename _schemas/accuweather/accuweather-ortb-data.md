---
description: OrtbData schema from AccuWeather API
layout: schema
name: OrtbData
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: extensions
  type: object
- description: ''
  name: segments
  type: array
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ortb-data-schema.json
slug: accuweather-ortb-data
source_filename: accuweather-ortb-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-data-schema.json\",\n  \"title\": \"OrtbData\",\n  \"description\": \"OrtbData schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"extensions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"nullable\": true\n      },\n      \"nullable\": true\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          }\n        },\n        \"additionalProperties\": false\n      },\n     \
  \ \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-data-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: OrtbData
---
