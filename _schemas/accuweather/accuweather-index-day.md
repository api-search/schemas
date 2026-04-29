---
description: IndexDay schema from AccuWeather API
layout: schema
name: IndexDay
properties_list:
- description: ''
  name: dayOfWeek
  type: string
- description: ''
  name: shortDayOfWeek
  type: string
- description: ''
  name: fullDayOfWeek
  type: string
- description: ''
  name: epoch
  type: integer
- description: ''
  name: dateTime
  type: string
- description: ''
  name: displayDate
  type: string
- description: ''
  name: longDisplayDate
  type: string
- description: ''
  name: value
  type: integer
- description: ''
  name: category
  type: string
- description: ''
  name: color
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-index-day-schema.json
slug: accuweather-index-day
source_filename: accuweather-index-day-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-index-day-schema.json\",\n  \"title\": \"IndexDay\",\n  \"description\": \"IndexDay schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"shortDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"fullDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"epoch\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"longDisplayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"\
  value\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-index-day-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: IndexDay
---
