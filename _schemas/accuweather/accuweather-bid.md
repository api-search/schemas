---
description: Bid schema from AccuWeather API
layout: schema
name: Bid
properties_list:
- description: ''
  name: bidder
  type: string
- description: ''
  name: params
  type: object
- description: ''
  name: isBuyItNow
  type: boolean
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-bid-schema.json
slug: accuweather-bid
source_filename: accuweather-bid-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-bid-schema.json\",\n  \"title\": \"Bid\",\n  \"description\": \"Bid schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bidder\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"params\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {},\n      \"nullable\": true\n    },\n    \"isBuyItNow\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-bid-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: Bid
---
