---
description: ExtendedForecastInformation schema from AccuWeather API
layout: schema
name: ExtendedForecastInformation
properties_list:
- description: ''
  name: ceiling
  type: string
- description: ''
  name: cloudCover
  type: string
- description: ''
  name: dewPoint
  type: string
- description: ''
  name: gusts
  type: string
- description: ''
  name: wind
  type: string
- description: ''
  name: windValue
  type: number
- description: ''
  name: windDegrees
  type: number
- description: ''
  name: windDirection
  type: string
- description: ''
  name: humidity
  type: string
- description: ''
  name: humidityValue
  type: integer
- description: ''
  name: indoorHumidity
  type: string
- description: ''
  name: indoorHumidityCategory
  type: string
- description: ''
  name: precipitation
  type: string
- description: ''
  name: pressure
  type: string
- description: ''
  name: ice
  type: string
- description: ''
  name: rain
  type: string
- description: ''
  name: snow
  type: string
- description: ''
  name: thunderstormProbability
  type: string
- description: ''
  name: uv
  type: object
- description: ''
  name: visibility
  type: string
- description: ''
  name: precipSummary
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-extended-forecast-information-schema.json
slug: accuweather-extended-forecast-information
source_filename: accuweather-extended-forecast-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-extended-forecast-information-schema.json\",\n  \"title\": \"ExtendedForecastInformation\",\n  \"description\": \"ExtendedForecastInformation schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ceiling\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"cloudCover\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"dewPoint\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"gusts\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"wind\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"windValue\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"windDegrees\": {\n      \"type\": \"number\",\n \
  \     \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"windDirection\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"humidity\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"humidityValue\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"indoorHumidity\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"indoorHumidityCategory\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"precipitation\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"pressure\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"ice\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"rain\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"snow\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"thunderstormProbability\": {\n     \
  \ \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"uv\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"format\": \"float\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"precipSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"past12Hours\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"past18Hours\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"past24Hours\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"past3Hours\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"past6Hours\": {\n          \"\
  type\": \"string\",\n          \"nullable\": true\n        },\n        \"past9Hours\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"pastHour\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-extended-forecast-information-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: ExtendedForecastInformation
---
