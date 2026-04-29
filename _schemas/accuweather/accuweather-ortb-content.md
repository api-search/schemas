---
description: OrtbContent schema from AccuWeather API
layout: schema
name: OrtbContent
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: categories
  type: array
- description: ''
  name: productQuality
  type: string
- description: ''
  name: context
  type: string
- description: ''
  name: keywords
  type: string
- description: ''
  name: sourceRelationship
  type: string
- description: ''
  name: language
  type: string
- description: ''
  name: data
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ortb-content-schema.json
slug: accuweather-ortb-content
source_filename: accuweather-ortb-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-content-schema.json\",\n  \"title\": \"OrtbContent\",\n  \"description\": \"OrtbContent schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    },\n    \"productQuality\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"keywords\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"sourceRelationship\": {\n      \"enum\": [\n        \"Indirect\",\n\
  \        \"Direct\"\n      ],\n      \"type\": \"string\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"extensions\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"nullable\": true\n          },\n          \"nullable\": true\n        },\n        \"segments\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              }\n            },\n            \"additionalProperties\": false\n          },\n          \"nullable\": true\n  \
  \      }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-content-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: OrtbContent
---
