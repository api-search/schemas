---
description: FavoriteLocation schema from AccuWeather API
layout: schema
name: FavoriteLocation
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
  name: displayTemperature
  type: string
- description: ''
  name: displayHighTemperature
  type: string
- description: ''
  name: displayLowTemperature
  type: string
- description: ''
  name: displayRealFeel
  type: string
- description: ''
  name: displayRealFeelShade
  type: string
- description: ''
  name: icon
  type: integer
- description: ''
  name: conditions
  type: string
- description: ''
  name: localTime
  type: string
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
  name: minuteCastForecast
  type: object
- description: ''
  name: numberOfAlerts
  type: integer
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-favorite-location-schema.json
slug: accuweather-favorite-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-favorite-location-schema.json\",\n  \"title\": \"FavoriteLocation\",\n  \"description\": \"FavoriteLocation schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"longName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayTemperature\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayHighTemperature\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayLowTemperature\"\
  : {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayRealFeel\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayRealFeelShade\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"icon\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"conditions\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"localTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isBefore7PM\": {\n      \"type\": \"boolean\"\n    },\n    \"isDayTime\": {\n      \"type\": \"boolean\"\n    },\n    \"minuteCastForecast\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"summary60\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"minutes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"\
  object\",\n            \"properties\": {\n              \"displayTime\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"minute\": {\n                \"type\": \"integer\",\n                \"format\": \"int32\"\n              },\n              \"color\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"dbz\": {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"nullable\": true\n              },\n              \"precipitationType\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              }\n            },\n            \"additionalProperties\": false\n          },\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"numberOfAlerts\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n\
  \    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-favorite-location-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: FavoriteLocation
---
