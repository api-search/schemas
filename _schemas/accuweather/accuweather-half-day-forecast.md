---
description: HalfDayForecast schema from AccuWeather API
layout: schema
name: HalfDayForecast
properties_list:
- description: ''
  name: temperature
  type: number
- description: ''
  name: displayTemperature
  type: string
- description: ''
  name: icon
  type: integer
- description: ''
  name: iconPhrase
  type: string
- description: ''
  name: phrase
  type: string
- description: ''
  name: longPhrase
  type: string
- description: ''
  name: precip
  type: string
- description: ''
  name: realFeelValue
  type: number
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-half-day-forecast-schema.json
slug: accuweather-half-day-forecast
source_filename: accuweather-half-day-forecast-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-half-day-forecast-schema.json\",\n  \"title\": \"HalfDayForecast\",\n  \"description\": \"HalfDayForecast schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"temperature\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"displayTemperature\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"icon\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"iconPhrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"phrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"longPhrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"precip\": {\n      \"type\": \"string\",\n      \"nullable\": true\n\
  \    },\n    \"realFeelValue\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-half-day-forecast-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: HalfDayForecast
---
