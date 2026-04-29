---
description: AirQuality schema from AccuWeather API
layout: schema
name: AirQuality
properties_list:
- description: ''
  name: category
  type: string
- description: ''
  name: categoryColor
  type: string
- description: ''
  name: date
  type: string
- description: ''
  name: dayOfWeek
  type: string
- description: ''
  name: dayOfWeekAbbreviated
  type: string
- description: ''
  name: displayDate
  type: string
- description: ''
  name: displayTime
  type: string
- description: ''
  name: dominantPollutant
  type: string
- description: ''
  name: hazardStatement
  type: string
- description: ''
  name: overallIndex
  type: number
- description: ''
  name: overallPlumeLabsIndex
  type: number
- description: ''
  name: pollutants
  type: array
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-air-quality-schema.json
slug: accuweather-air-quality
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-air-quality-schema.json\",\n  \"title\": \"AirQuality\",\n  \"description\": \"AirQuality schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"categoryColor\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"dayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"dayOfWeekAbbreviated\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n  \
  \  },\n    \"dominantPollutant\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hazardStatement\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"overallIndex\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"overallPlumeLabsIndex\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"pollutants\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"concentration\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"index\": {\n            \"type\": \"number\",\n            \"format\": \"double\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"source\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"type\": {\n            \"type\": \"string\"\
  ,\n            \"nullable\": true\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-air-quality-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: AirQuality
---
