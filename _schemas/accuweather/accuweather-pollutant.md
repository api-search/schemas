---
description: Pollutant schema from AccuWeather API
layout: schema
name: Pollutant
properties_list:
- description: ''
  name: concentration
  type: string
- description: ''
  name: index
  type: number
- description: ''
  name: name
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: type
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-pollutant-schema.json
slug: accuweather-pollutant
source_filename: accuweather-pollutant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-pollutant-schema.json\",\n  \"title\": \"Pollutant\",\n  \"description\": \"Pollutant schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"concentration\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"index\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-pollutant-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: Pollutant
---
