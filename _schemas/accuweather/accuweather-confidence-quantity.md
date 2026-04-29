---
description: ConfidenceQuantity schema from AccuWeather API
layout: schema
name: ConfidenceQuantity
properties_list:
- description: ''
  name: value
  type: number
- description: ''
  name: unit
  type: string
- description: ''
  name: unitType
  type: integer
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-confidence-quantity-schema.json
slug: accuweather-confidence-quantity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-confidence-quantity-schema.json\",\n  \"title\": \"ConfidenceQuantity\",\n  \"description\": \"ConfidenceQuantity schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"unitType\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-confidence-quantity-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: ConfidenceQuantity
---
