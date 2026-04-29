---
description: Storm schema from AccuWeather API
layout: schema
name: Storm
properties_list:
- description: ''
  name: accuId
  type: integer
- description: ''
  name: eventKey
  type: string
- description: ''
  name: isActive
  type: boolean
- description: ''
  name: basin
  type: string
- description: ''
  name: basinId
  type: string
- description: ''
  name: basinSlug
  type: string
- description: ''
  name: governmentId
  type: integer
- description: ''
  name: level
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: updatedStormName
  type: string
- description: ''
  name: stormPositions
  type: array
- description: ''
  name: peakPosition
  type: object
- description: ''
  name: start
  type: string
- description: ''
  name: startEpoch
  type: integer
- description: ''
  name: end
  type: string
- description: ''
  name: localStart
  type: string
- description: ''
  name: localEnd
  type: string
- description: ''
  name: year
  type: integer
- description: ''
  name: isFuture
  type: boolean
- description: ''
  name: stormLink
  type: string
- description: ''
  name: localizedStartDate
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-storm-schema.json
slug: accuweather-storm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-storm-schema.json\",\n  \"title\": \"Storm\",\n  \"description\": \"Storm schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accuId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"eventKey\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    },\n    \"basin\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"readOnly\": true\n    },\n    \"basinId\": {\n      \"enum\": [\n        \"AL\",\n        \"EP\",\n        \"SI\",\n        \"NI\",\n        \"CP\",\n        \"NP\",\n        \"SP\"\n      ],\n      \"type\": \"string\"\n    },\n    \"basinSlug\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n \
  \   \"governmentId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"updatedStormName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"stormPositions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"coordinates\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"coordinates\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\"\
  : \"number\",\n                      \"format\": \"double\"\n                    }\n                  }\n                },\n                \"nullable\": true\n              }\n            },\n            \"additionalProperties\": false\n          },\n          \"dateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"nullable\": true\n          },\n          \"localDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"nullable\": true\n          },\n          \"localDayOfWeek\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"dateTimeLabelShort\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"dateTimeLabel\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"shortDateShortTimeLabel\": {\n            \"type\": \"string\",\n            \"nullable\": true\n\
  \          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"isCurrent\": {\n            \"type\": \"boolean\",\n            \"nullable\": true\n          },\n          \"isHistorical\": {\n            \"type\": \"boolean\",\n            \"nullable\": true\n          },\n          \"isMarked\": {\n            \"type\": \"boolean\"\n          },\n          \"isPeak\": {\n            \"type\": \"boolean\",\n            \"nullable\": true\n          },\n          \"latitude\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"nullable\": true\n          },\n          \"longitude\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"nullable\": true\n          },\n          \"maximumSustainedWind\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"maximumSustainedWindValue\": {\n            \"\
  type\": \"number\",\n            \"format\": \"float\",\n            \"nullable\": true\n          },\n          \"maximumWindGust\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"maximumWindGustValue\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"nullable\": true\n          },\n          \"windDegrees\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"nullable\": true\n          },\n          \"minimumPressure\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"position\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"speed\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"localizedStatus\": {\n          \
  \  \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"statusName\": {\n            \"type\": \"string\",\n            \"nullable\": true,\n            \"readOnly\": true\n          },\n          \"statusIcon\": {\n            \"enum\": [\n              \"ExtratropicalStorm\",\n              \"Subtropical\",\n              \"Category0\",\n              \"Category1\",\n              \"Category2\",\n              \"Category3\",\n              \"Category4\",\n              \"Category5\",\n              \"TropicalRainStorm\",\n              \"TropicalDepression\"\n            ],\n            \"type\": \"string\"\n          },\n          \"statusIconString\": {\n            \"type\": \"string\",\n            \"nullable\": true,\n            \"readOnly\": true\n          },\n          \"landmarkReferences\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"landmark\"\
  : {\n                  \"type\": \"string\",\n                  \"nullable\": true\n                },\n                \"distance\": {\n                  \"type\": \"string\",\n                  \"nullable\": true\n                }\n              },\n              \"additionalProperties\": false\n            },\n            \"nullable\": true\n          },\n          \"eventKey\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"nullable\": true\n    },\n    \"peakPosition\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coordinates\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"coordinates\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"array\",\n                \"\
  items\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"number\",\n                    \"format\": \"double\"\n                  }\n                }\n              },\n              \"nullable\": true\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"dateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"nullable\": true\n        },\n        \"localDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"nullable\": true\n        },\n        \"localDayOfWeek\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"dateTimeLabelShort\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"dateTimeLabel\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"shortDateShortTimeLabel\": {\n          \"type\"\
  : \"string\",\n          \"nullable\": true\n        },\n        \"direction\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"isCurrent\": {\n          \"type\": \"boolean\",\n          \"nullable\": true\n        },\n        \"isHistorical\": {\n          \"type\": \"boolean\",\n          \"nullable\": true\n        },\n        \"isMarked\": {\n          \"type\": \"boolean\"\n        },\n        \"isPeak\": {\n          \"type\": \"boolean\",\n          \"nullable\": true\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"maximumSustainedWind\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"maximumSustainedWindValue\": {\n          \"type\": \"number\",\n       \
  \   \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"maximumWindGust\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"maximumWindGustValue\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"windDegrees\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"nullable\": true\n        },\n        \"minimumPressure\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"position\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"speed\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"localizedStatus\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"statusName\": {\n   \
  \       \"type\": \"string\",\n          \"nullable\": true,\n          \"readOnly\": true\n        },\n        \"statusIcon\": {\n          \"enum\": [\n            \"ExtratropicalStorm\",\n            \"Subtropical\",\n            \"Category0\",\n            \"Category1\",\n            \"Category2\",\n            \"Category3\",\n            \"Category4\",\n            \"Category5\",\n            \"TropicalRainStorm\",\n            \"TropicalDepression\"\n          ],\n          \"type\": \"string\"\n        },\n        \"statusIconString\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"readOnly\": true\n        },\n        \"landmarkReferences\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"landmark\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"distance\": {\n                \"type\": \"string\"\
  ,\n                \"nullable\": true\n              }\n            },\n            \"additionalProperties\": false\n          },\n          \"nullable\": true\n        },\n        \"eventKey\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"startEpoch\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"localStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"localEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n   \
  \ \"isFuture\": {\n      \"type\": \"boolean\"\n    },\n    \"stormLink\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"localizedStartDate\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-storm-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: Storm
---
