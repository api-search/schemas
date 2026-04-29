---
description: WeatherInfo schema from AccuWeather API
layout: schema
name: WeatherInfo
properties_list:
- description: Surefind location key for the user's weather location Eg. 335315
  name: key
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-weather-info-schema.json
slug: accuweather-weather-info
source_filename: accuweather-weather-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-weather-info-schema.json\",\n  \"title\": \"WeatherInfo\",\n  \"description\": \"WeatherInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Surefind location key for the user's weather location\\r\\nEg. 335315\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-weather-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: WeatherInfo
---
