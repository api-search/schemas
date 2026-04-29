---
description: SessionInfo schema from AccuWeather API
layout: schema
name: SessionInfo
properties_list:
- description: Unique ID for the user's session (persistent to 10m after the last pageview)
  name: id
  type: string
- description: Unique ID for the partner from the URL
  name: partner
  type: string
- description: ''
  name: utm
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-session-info-schema.json
slug: accuweather-session-info
source_filename: accuweather-session-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-session-info-schema.json\",\n  \"title\": \"SessionInfo\",\n  \"description\": \"SessionInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for the user's session (persistent to 10m after the last pageview)\",\n      \"nullable\": true\n    },\n    \"partner\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for the partner from the URL\",\n      \"nullable\": true\n    },\n    \"utm\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"utm_source from the URL\",\n          \"nullable\": true\n        },\n        \"medium\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"utm_medium from the URL\",\n          \"nullable\": true\n        },\n        \"campaign\": {\n          \"type\": \"string\",\n          \"description\": \"utm_campaign from the URL\",\n          \"nullable\": true\n        },\n        \"term\": {\n          \"type\": \"string\",\n          \"description\": \"utm_term from the URL\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-session-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: SessionInfo
---
