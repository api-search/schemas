---
description: 'ISO 15143-3 vehicle telemetry payload returned by the CNH FieldOps API. Two profiles are supported: CP (CAN Parameter) and MH (Machine Health).'
layout: schema
name: CNH FieldOps Vehicle Telemetry
properties_list:
- description: ''
  name: vehicleId
  type: string
- description: CP = CAN Parameter profile (default). MH = Machine Health profile.
  name: profile
  type: string
- description: ''
  name: windowStart
  type: string
- description: ''
  name: windowEnd
  type: string
- description: ''
  name: location
  type: object
- description: Engine operating hours over the window.
  name: operatingHours
  type: number
- description: Engine idle hours over the window.
  name: idleHours
  type: number
- description: Fraction of tank fuel remaining at end of window.
  name: fuelRemainingRatio
  type: number
- description: Diesel Exhaust Fluid remaining (liters).
  name: defRemaining
  type: number
- description: Peak ground speed observed during the window (km/h).
  name: peakDailySpeed
  type: number
- description: Total distance travelled in the window (km).
  name: distance
  type: number
- description: Comma-separated error/quality tags (e.g. NO_GPS_FIX, NULL_DATA, UNREALISTIC_VALUE).
  name: errorTags
  type: string
- description: ''
  name: faultCodes
  type: array
provider_name: CNH
provider_slug: cnh
schema_file: json-schema/cnh-telemetry-schema.json
slug: cnh-telemetry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cnh/main/json-schema/cnh-telemetry-schema.json\",\n  \"title\": \"CNH FieldOps Vehicle Telemetry\",\n  \"description\": \"ISO 15143-3 vehicle telemetry payload returned by the CNH FieldOps API. Two profiles are supported: CP (CAN Parameter) and MH (Machine Health).\",\n  \"type\": \"object\",\n  \"required\": [\"vehicleId\", \"profile\"],\n  \"properties\": {\n    \"vehicleId\": { \"type\": \"string\" },\n    \"profile\": {\n      \"type\": \"string\",\n      \"enum\": [\"CP\", \"MH\"],\n      \"description\": \"CP = CAN Parameter profile (default). MH = Machine Health profile.\"\n    },\n    \"windowStart\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"windowEnd\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"latitude\": { \"type\": \"number\"\
  \ },\n        \"longitude\": { \"type\": \"number\" },\n        \"altitude\": { \"type\": \"number\" },\n        \"gpsFix\": { \"type\": \"boolean\" }\n      }\n    },\n    \"operatingHours\": {\n      \"type\": \"number\",\n      \"description\": \"Engine operating hours over the window.\"\n    },\n    \"idleHours\": {\n      \"type\": \"number\",\n      \"description\": \"Engine idle hours over the window.\"\n    },\n    \"fuelRemainingRatio\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Fraction of tank fuel remaining at end of window.\"\n    },\n    \"defRemaining\": {\n      \"type\": \"number\",\n      \"description\": \"Diesel Exhaust Fluid remaining (liters).\"\n    },\n    \"peakDailySpeed\": {\n      \"type\": \"number\",\n      \"description\": \"Peak ground speed observed during the window (km/h).\"\n    },\n    \"distance\": {\n      \"type\": \"number\",\n      \"description\": \"Total distance travelled in the window\
  \ (km).\"\n    },\n    \"errorTags\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated error/quality tags (e.g. NO_GPS_FIX, NULL_DATA, UNREALISTIC_VALUE).\"\n    },\n    \"faultCodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": { \"type\": \"string\" },\n          \"severity\": {\n            \"type\": \"string\",\n            \"enum\": [\"INFO\", \"WARNING\", \"FAULT\"]\n          },\n          \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\" },\n          \"description\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/json-schema/cnh-telemetry-schema.json
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
title: CNH FieldOps Vehicle Telemetry
---
