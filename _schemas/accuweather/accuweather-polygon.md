---
description: Polygon schema from AccuWeather API
layout: schema
name: Polygon
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: coordinates
  type: array
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-polygon-schema.json
slug: accuweather-polygon
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-polygon-schema.json\",\n  \"title\": \"Polygon\",\n  \"description\": \"Polygon schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"coordinates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"number\",\n            \"format\": \"double\"\n          }\n        }\n      },\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-polygon-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: Polygon
---
