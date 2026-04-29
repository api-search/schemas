---
description: UVIndex schema from AccuWeather API
layout: schema
name: UVIndex
properties_list:
- description: ''
  name: category
  type: string
- description: ''
  name: value
  type: number
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-uv-index-schema.json
slug: accuweather-uv-index
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-uv-index-schema.json\",\n  \"title\": \"UVIndex\",\n  \"description\": \"UVIndex schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"format\": \"float\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-uv-index-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: UVIndex
---
