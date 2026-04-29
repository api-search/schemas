---
description: DeviceInfo schema from AccuWeather API
layout: schema
name: DeviceInfo
properties_list:
- description: Name of the user's browser. Eg. 'Chrome'
  name: name
  type: string
- description: Name of the user's device maker. Eg. 'Apple' or 'Samsung'
  name: brand
  type: string
- description: Version of the user's browser. Eg. '16'
  name: version
  type: string
- description: One of 'mobile', 'tablet', or 'desktop'
  name: category
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-device-info-schema.json
slug: accuweather-device-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-device-info-schema.json\",\n  \"title\": \"DeviceInfo\",\n  \"description\": \"DeviceInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the user's browser.\\r\\nEg. 'Chrome'\",\n      \"nullable\": true\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the user's device maker.\\r\\nEg. 'Apple' or 'Samsung'\",\n      \"nullable\": true\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the user's browser.\\r\\nEg. '16'\",\n      \"nullable\": true\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"One of 'mobile', 'tablet', or 'desktop'\",\n      \"nullable\": true\n    }\n\
  \  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-device-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: DeviceInfo
---
