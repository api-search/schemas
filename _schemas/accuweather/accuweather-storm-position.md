---
description: StormPosition schema from AccuWeather API
layout: schema
name: StormPosition
properties_list:
- description: ''
  name: coordinates
  type: object
- description: ''
  name: dateTime
  type: string
- description: ''
  name: localDate
  type: string
- description: ''
  name: localDayOfWeek
  type: string
- description: ''
  name: dateTimeLabelShort
  type: string
- description: ''
  name: dateTimeLabel
  type: string
- description: ''
  name: shortDateShortTimeLabel
  type: string
- description: ''
  name: direction
  type: string
- description: ''
  name: isCurrent
  type: boolean
- description: ''
  name: isHistorical
  type: boolean
- description: ''
  name: isMarked
  type: boolean
- description: ''
  name: isPeak
  type: boolean
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
- description: ''
  name: maximumSustainedWind
  type: string
- description: ''
  name: maximumSustainedWindValue
  type: number
- description: ''
  name: maximumWindGust
  type: string
- description: ''
  name: maximumWindGustValue
  type: number
- description: ''
  name: windDegrees
  type: number
- description: ''
  name: minimumPressure
  type: string
- description: ''
  name: position
  type: string
- description: ''
  name: speed
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: localizedStatus
  type: string
- description: ''
  name: statusName
  type: string
- description: ''
  name: statusIcon
  type: string
- description: ''
  name: statusIconString
  type: string
- description: ''
  name: landmarkReferences
  type: array
- description: ''
  name: eventKey
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-storm-position-schema.json
slug: accuweather-storm-position
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-storm-position-schema.json\",\n  \"title\": \"StormPosition\",\n  \"description\": \"StormPosition schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coordinates\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"coordinates\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"number\",\n                \"format\": \"double\"\n              }\n            }\n          },\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"dateTime\": {\n \
  \     \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"localDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"localDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"dateTimeLabelShort\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"dateTimeLabel\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"shortDateShortTimeLabel\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isCurrent\": {\n      \"type\": \"boolean\",\n      \"nullable\": true\n    },\n    \"isHistorical\": {\n      \"type\": \"boolean\",\n      \"nullable\": true\n    },\n    \"isMarked\": {\n      \"type\": \"boolean\"\n    },\n    \"isPeak\": {\n      \"type\": \"boolean\",\n      \"nullable\": true\n    },\n    \"latitude\"\
  : {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"maximumSustainedWind\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"maximumSustainedWindValue\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"maximumWindGust\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"maximumWindGustValue\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"windDegrees\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"minimumPressure\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"speed\": {\n      \"type\": \"string\",\n \
  \     \"nullable\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"localizedStatus\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"statusName\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"readOnly\": true\n    },\n    \"statusIcon\": {\n      \"enum\": [\n        \"ExtratropicalStorm\",\n        \"Subtropical\",\n        \"Category0\",\n        \"Category1\",\n        \"Category2\",\n        \"Category3\",\n        \"Category4\",\n        \"Category5\",\n        \"TropicalRainStorm\",\n        \"TropicalDepression\"\n      ],\n      \"type\": \"string\"\n    },\n    \"statusIconString\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"readOnly\": true\n    },\n    \"landmarkReferences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"landmark\": {\n            \"type\": \"string\",\n      \
  \      \"nullable\": true\n          },\n          \"distance\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"nullable\": true\n    },\n    \"eventKey\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-storm-position-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: StormPosition
---
