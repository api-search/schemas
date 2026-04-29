---
description: PageInfo schema from AccuWeather API
layout: schema
name: PageInfo
properties_list:
- description: Page group like 'three-day' or 'hourly' designating the page category
  name: group
  type: string
- description: URL of the page
  name: url
  type: string
- description: Referrer of the page
  name: referrer
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-page-info-schema.json
slug: accuweather-page-info
source_filename: accuweather-page-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-page-info-schema.json\",\n  \"title\": \"PageInfo\",\n  \"description\": \"PageInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"Page group like 'three-day' or 'hourly' designating the page category\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the page\",\n      \"nullable\": true\n    },\n    \"referrer\": {\n      \"type\": \"string\",\n      \"description\": \"Referrer of the page\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-page-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: PageInfo
---
