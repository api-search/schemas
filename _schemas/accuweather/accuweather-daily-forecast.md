---
description: DailyForecast schema from AccuWeather API
layout: schema
name: DailyForecast
properties_list:
- description: ''
  name: dayOfWeek
  type: string
- description: ''
  name: shortDayOfWeek
  type: string
- description: ''
  name: fullDayOfWeek
  type: string
- description: ''
  name: epoch
  type: integer
- description: ''
  name: dateTime
  type: string
- description: ''
  name: displayDate
  type: string
- description: ''
  name: longDisplayDate
  type: string
- description: ''
  name: hasAlert
  type: boolean
- description: ''
  name: day
  type: object
- description: ''
  name: night
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-daily-forecast-schema.json
slug: accuweather-daily-forecast
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-daily-forecast-schema.json\",\n  \"title\": \"DailyForecast\",\n  \"description\": \"DailyForecast schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"shortDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"fullDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"epoch\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"longDisplayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n\
  \    },\n    \"hasAlert\": {\n      \"type\": \"boolean\"\n    },\n    \"day\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"temperature\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"displayTemperature\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"icon\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        },\n        \"iconPhrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"longPhrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"precip\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"realFeelValue\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\"\
  : true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"night\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"temperature\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"displayTemperature\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"icon\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        },\n        \"iconPhrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"longPhrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"precip\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"realFeelValue\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n       \
  \   \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-daily-forecast-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: DailyForecast
---
