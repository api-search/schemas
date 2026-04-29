---
description: Real-time telematics data from an AGCO machine.
layout: schema
name: Telemetry
properties_list:
- description: Machine identifier.
  name: machine_id
  type: string
- description: Data collection timestamp.
  name: timestamp
  type: string
- description: Engine RPM.
  name: engine_speed
  type: number
- description: Engine load percentage.
  name: engine_load
  type: number
- description: Cumulative engine hours.
  name: engine_hours
  type: number
- description: Fuel level percentage.
  name: fuel_level
  type: number
- description: Fuel consumption in liters/hour.
  name: fuel_consumption_rate
  type: number
- description: Ground speed in km/h.
  name: ground_speed
  type: number
- description: Engine coolant temperature in Celsius.
  name: coolant_temperature
  type: number
- description: Active diagnostic fault codes.
  name: fault_codes
  type: array
- description: Current machine operating mode.
  name: operating_mode
  type: string
provider_name: agco
provider_slug: agco
schema_file: json-schema/agco-telemetry-schema.json
slug: agco-telemetry
source_filename: agco-telemetry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/json-schema/agco-telemetry-schema.json\",\n  \"title\": \"Telemetry\",\n  \"description\": \"Real-time telematics data from an AGCO machine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"machine_id\": {\n      \"type\": \"string\",\n      \"description\": \"Machine identifier.\",\n      \"example\": \"mach-500123\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Data collection timestamp.\",\n      \"example\": \"2025-04-01T10:30:00Z\"\n    },\n    \"engine_speed\": {\n      \"type\": \"number\",\n      \"description\": \"Engine RPM.\",\n      \"example\": 1850\n    },\n    \"engine_load\": {\n      \"type\": \"number\",\n      \"description\": \"Engine load percentage.\",\n      \"example\": 75.2\n    },\n    \"engine_hours\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"Cumulative engine hours.\",\n      \"example\": 1250.5\n    },\n    \"fuel_level\": {\n      \"type\": \"number\",\n      \"description\": \"Fuel level percentage.\",\n      \"example\": 78.5\n    },\n    \"fuel_consumption_rate\": {\n      \"type\": \"number\",\n      \"description\": \"Fuel consumption in liters/hour.\",\n      \"example\": 22.3\n    },\n    \"ground_speed\": {\n      \"type\": \"number\",\n      \"description\": \"Ground speed in km/h.\",\n      \"example\": 8.5\n    },\n    \"coolant_temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Engine coolant temperature in Celsius.\",\n      \"example\": 85.0\n    },\n    \"fault_codes\": {\n      \"type\": \"array\",\n      \"description\": \"Active diagnostic fault codes.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": []\n    },\n    \"operating_mode\": {\n      \"type\": \"string\",\n      \"description\": \"Current machine operating\
  \ mode.\",\n      \"example\": \"field_work\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/json-schema/agco-telemetry-schema.json
tags: []
title: Telemetry
---
