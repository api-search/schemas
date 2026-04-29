---
description: LandmarkReference schema from AccuWeather API
layout: schema
name: LandmarkReference
properties_list:
- description: ''
  name: landmark
  type: string
- description: ''
  name: distance
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-landmark-reference-schema.json
slug: accuweather-landmark-reference
source_filename: accuweather-landmark-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-landmark-reference-schema.json\",\n  \"title\": \"LandmarkReference\",\n  \"description\": \"LandmarkReference schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"landmark\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"distance\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-landmark-reference-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: LandmarkReference
---
