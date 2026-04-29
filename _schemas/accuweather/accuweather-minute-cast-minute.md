---
description: MinuteCastMinute schema from AccuWeather API
layout: schema
name: MinuteCastMinute
properties_list:
- description: ''
  name: displayTime
  type: string
- description: ''
  name: minute
  type: integer
- description: ''
  name: color
  type: string
- description: ''
  name: dbz
  type: number
- description: ''
  name: precipitationType
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-minute-cast-minute-schema.json
slug: accuweather-minute-cast-minute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-minute-cast-minute-schema.json\",\n  \"title\": \"MinuteCastMinute\",\n  \"description\": \"MinuteCastMinute schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"minute\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"dbz\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"precipitationType\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-minute-cast-minute-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: MinuteCastMinute
---
