---
description: OrtbPublisher schema from AccuWeather API
layout: schema
name: OrtbPublisher
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: domain
  type: string
- description: ''
  name: categories
  type: array
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ortb-publisher-schema.json
slug: accuweather-ortb-publisher
source_filename: accuweather-ortb-publisher-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-publisher-schema.json\",\n  \"title\": \"OrtbPublisher\",\n  \"description\": \"OrtbPublisher schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-publisher-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: OrtbPublisher
---
