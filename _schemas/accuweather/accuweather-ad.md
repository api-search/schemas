---
description: Ad schema from AccuWeather API
layout: schema
name: Ad
properties_list:
- description: ''
  name: slot
  type: string
- description: ''
  name: adDivId
  type: string
- description: ''
  name: adUnitCode
  type: string
- description: ''
  name: bidders
  type: array
- description: ''
  name: upr
  type: number
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ad-schema.json
slug: accuweather-ad
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ad-schema.json\",\n  \"title\": \"Ad\",\n  \"description\": \"Ad schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"slot\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"adDivId\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"adUnitCode\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"bidders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"bidder\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"params\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {},\n            \"nullable\": true\n          },\n          \"isBuyItNow\": {\n  \
  \          \"type\": \"boolean\"\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"nullable\": true\n    },\n    \"upr\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ad-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: Ad
---
