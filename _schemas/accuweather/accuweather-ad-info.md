---
description: AdInfo schema from AccuWeather API
layout: schema
name: AdInfo
properties_list:
- description: Simplified ad code for ad slots on the page. Eg. '6581/web/us/*/news_info/country_home'
  name: code
  type: string
- description: One of 'active', 'missing', or 'restricted' indicating a user's ID status Default missing.
  name: status
  type: string
- description: One of 'active', 'missing', or 'restricted' indicating a user can access 3rd party cookies or not. Default missing.
  name: cookie3p
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ad-info-schema.json
slug: accuweather-ad-info
source_filename: accuweather-ad-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ad-info-schema.json\",\n  \"title\": \"AdInfo\",\n  \"description\": \"AdInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Simplified ad code for ad slots on the page.\\r\\nEg. '6581/web/us/*/news_info/country_home'\",\n      \"nullable\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"One of 'active', 'missing', or 'restricted' indicating a user's ID status\\r\\nDefault missing.\",\n      \"nullable\": true\n    },\n    \"cookie3p\": {\n      \"type\": \"string\",\n      \"description\": \"One of 'active', 'missing', or 'restricted' indicating a user can access 3rd party cookies or not.\\r\\nDefault missing.\",\n      \"nullable\": true\n    }\n  },\n\
  \  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ad-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: AdInfo
---
