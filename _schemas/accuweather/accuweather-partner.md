---
description: Partner schema from AccuWeather API
layout: schema
name: Partner
properties_list:
- description: ''
  name: siteName
  type: string
- description: ''
  name: logo
  type: string
- description: ''
  name: link
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-partner-schema.json
slug: accuweather-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-partner-schema.json\",\n  \"title\": \"Partner\",\n  \"description\": \"Partner schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"siteName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-partner-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: Partner
---
