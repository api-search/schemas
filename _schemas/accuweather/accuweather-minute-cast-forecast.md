---
description: MinuteCastForecast schema from AccuWeather API
layout: schema
name: MinuteCastForecast
properties_list:
- description: ''
  name: summary60
  type: string
- description: ''
  name: minutes
  type: array
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-minute-cast-forecast-schema.json
slug: accuweather-minute-cast-forecast
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-minute-cast-forecast-schema.json\",\n  \"title\": \"MinuteCastForecast\",\n  \"description\": \"MinuteCastForecast schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summary60\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"minutes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayTime\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"minute\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"color\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"dbz\": {\n            \"type\": \"number\",\n            \"format\"\
  : \"float\",\n            \"nullable\": true\n          },\n          \"precipitationType\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-minute-cast-forecast-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: MinuteCastForecast
---
