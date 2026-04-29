---
description: RecentLocation schema from AccuWeather API
layout: schema
name: RecentLocation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: longName
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: localTime
  type: string
- description: ''
  name: displayTemperature
  type: string
- description: ''
  name: icon
  type: integer
- description: ''
  name: color
  type: string
- description: ''
  name: isBefore7PM
  type: boolean
- description: ''
  name: isDayTime
  type: boolean
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-recent-location-schema.json
slug: accuweather-recent-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-recent-location-schema.json\",\n  \"title\": \"RecentLocation\",\n  \"description\": \"RecentLocation schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"longName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"localTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayTemperature\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"icon\": {\n      \"type\": \"integer\"\
  ,\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isBefore7PM\": {\n      \"type\": \"boolean\"\n    },\n    \"isDayTime\": {\n      \"type\": \"boolean\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-recent-location-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: RecentLocation
---
