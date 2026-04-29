---
description: UTMInfo schema from AccuWeather API
layout: schema
name: UTMInfo
properties_list:
- description: utm_source from the URL
  name: source
  type: string
- description: utm_medium from the URL
  name: medium
  type: string
- description: utm_campaign from the URL
  name: campaign
  type: string
- description: utm_term from the URL
  name: term
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-utm-info-schema.json
slug: accuweather-utm-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-utm-info-schema.json\",\n  \"title\": \"UTMInfo\",\n  \"description\": \"UTMInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"utm_source from the URL\",\n      \"nullable\": true\n    },\n    \"medium\": {\n      \"type\": \"string\",\n      \"description\": \"utm_medium from the URL\",\n      \"nullable\": true\n    },\n    \"campaign\": {\n      \"type\": \"string\",\n      \"description\": \"utm_campaign from the URL\",\n      \"nullable\": true\n    },\n    \"term\": {\n      \"type\": \"string\",\n      \"description\": \"utm_term from the URL\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-utm-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: UTMInfo
---
