---
description: CurrentConditions schema from AccuWeather API
layout: schema
name: CurrentConditions
properties_list:
- description: ''
  name: extended
  type: object
- description: ''
  name: isDayTime
  type: boolean
- description: ''
  name: iconCode
  type: integer
- description: ''
  name: now
  type: string
- description: ''
  name: phrase
  type: string
- description: ''
  name: realFeel
  type: string
- description: ''
  name: realFeelShade
  type: string
- description: ''
  name: temperature
  type: string
- description: ''
  name: temperatureValue
  type: number
- description: ''
  name: realFeelValue
  type: number
- description: ''
  name: realFeelShadeValue
  type: number
- description: ''
  name: realFeelPhrase
  type: string
- description: ''
  name: realFeelShadePhrase
  type: string
- description: ''
  name: apparentTempImperial
  type: number
- description: ''
  name: windSpeedImperial
  type: number
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-current-conditions-schema.json
slug: accuweather-current-conditions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-current-conditions-schema.json\",\n  \"title\": \"CurrentConditions\",\n  \"description\": \"CurrentConditions schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"extended\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ceiling\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"cloudCover\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"dewPoint\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"gusts\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"wind\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"windValue\": {\n          \"type\": \"\
  number\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"windDegrees\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"windDirection\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"humidity\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"humidityValue\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"indoorHumidity\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"indoorHumidityCategory\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"precipitation\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"pressure\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n   \
  \     \"ice\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"rain\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"snow\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"thunderstormProbability\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"uv\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"category\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"visibility\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"precipSummary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"past12Hours\"\
  : {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past18Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past24Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past3Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past6Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past9Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"pastHour\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            }\n          },\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"isDayTime\": {\n      \"type\": \"boolean\"\n    },\n    \"iconCode\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"now\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"phrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"realFeel\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"realFeelShade\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"temperature\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"temperatureValue\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"realFeelValue\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"realFeelShadeValue\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"realFeelPhrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"realFeelShadePhrase\": {\n      \"type\": \"string\"\
  ,\n      \"nullable\": true\n    },\n    \"apparentTempImperial\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"windSpeedImperial\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-current-conditions-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: CurrentConditions
---
