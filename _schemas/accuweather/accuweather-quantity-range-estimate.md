---
description: QuantityRangeEstimate schema from AccuWeather API
layout: schema
name: QuantityRangeEstimate
properties_list:
- description: ''
  name: displayAmount
  type: string
- description: ''
  name: low
  type: object
- description: ''
  name: high
  type: object
- description: ''
  name: probability
  type: integer
- description: ''
  name: phrase
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-quantity-range-estimate-schema.json
slug: accuweather-quantity-range-estimate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-quantity-range-estimate-schema.json\",\n  \"title\": \"QuantityRangeEstimate\",\n  \"description\": \"QuantityRangeEstimate schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayAmount\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"low\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"unitType\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"high\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"value\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"unitType\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"probability\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"phrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-quantity-range-estimate-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: QuantityRangeEstimate
---
