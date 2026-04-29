---
description: HourlyForecast schema from AccuWeather API
layout: schema
name: HourlyForecast
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
  name: icon
  type: integer
- description: ''
  name: temperature
  type: string
- description: ''
  name: precip
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
  name: isDayLight
  type: boolean
- description: ''
  name: extended
  type: object
- description: ''
  name: airQuality
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-hourly-forecast-schema.json
slug: accuweather-hourly-forecast
source_filename: accuweather-hourly-forecast-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-hourly-forecast-schema.json\",\n  \"title\": \"HourlyForecast\",\n  \"description\": \"HourlyForecast schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"shortDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"fullDayOfWeek\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"epoch\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"displayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"longDisplayDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n\
  \    },\n    \"hasAlert\": {\n      \"type\": \"boolean\"\n    },\n    \"icon\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"temperature\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"precip\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"phrase\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"realFeel\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"realFeelShade\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isDayLight\": {\n      \"type\": \"boolean\"\n    },\n    \"extended\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ceiling\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"cloudCover\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"dewPoint\": {\n          \"type\": \"string\",\n          \"nullable\": true\n\
  \        },\n        \"gusts\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"wind\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"windValue\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"windDegrees\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"windDirection\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"humidity\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"humidityValue\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"indoorHumidity\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"indoorHumidityCategory\": {\n          \"type\": \"string\"\
  ,\n          \"nullable\": true\n        },\n        \"precipitation\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"pressure\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"ice\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"rain\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"snow\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"thunderstormProbability\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"uv\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"category\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\"\n            }\n          },\n          \"additionalProperties\"\
  : false\n        },\n        \"visibility\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"precipSummary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"past12Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past18Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past24Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past3Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past6Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"past9Hours\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"pastHour\": {\n              \"type\": \"string\",\n       \
  \       \"nullable\": true\n            }\n          },\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"airQuality\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"categoryColor\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"nullable\": true\n        },\n        \"dayOfWeek\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"dayOfWeekAbbreviated\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"displayDate\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"displayTime\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n\
  \        \"dominantPollutant\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"hazardStatement\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"overallIndex\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        },\n        \"overallPlumeLabsIndex\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        },\n        \"pollutants\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"concentration\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"index\": {\n                \"type\": \"number\",\n                \"format\": \"double\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"source\": {\n     \
  \           \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              }\n            },\n            \"additionalProperties\": false\n          },\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-hourly-forecast-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: HourlyForecast
---
