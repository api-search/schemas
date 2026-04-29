---
description: PrecipitationSummary schema from AccuWeather API
layout: schema
name: PrecipitationSummary
properties_list:
- description: ''
  name: past12Hours
  type: string
- description: ''
  name: past18Hours
  type: string
- description: ''
  name: past24Hours
  type: string
- description: ''
  name: past3Hours
  type: string
- description: ''
  name: past6Hours
  type: string
- description: ''
  name: past9Hours
  type: string
- description: ''
  name: pastHour
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-precipitation-summary-schema.json
slug: accuweather-precipitation-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-precipitation-summary-schema.json\",\n  \"title\": \"PrecipitationSummary\",\n  \"description\": \"PrecipitationSummary schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"past12Hours\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"past18Hours\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"past24Hours\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"past3Hours\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"past6Hours\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"past9Hours\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"pastHour\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n\
  \  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-precipitation-summary-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: PrecipitationSummary
---
