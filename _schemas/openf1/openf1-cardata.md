---
description: ''
layout: schema
name: OpenF1 Car Telemetry
properties_list:
- description: ''
  name: meeting_key
  type: integer
- description: ''
  name: session_key
  type: integer
- description: ''
  name: driver_number
  type: integer
- description: ''
  name: date
  type: string
- description: ''
  name: rpm
  type: integer
- description: ''
  name: speed
  type: integer
- description: ''
  name: n_gear
  type: integer
- description: ''
  name: throttle
  type: integer
- description: ''
  name: brake
  type: integer
- description: ''
  name: drs
  type: integer
provider_name: OpenF1
provider_slug: openf1
schema_file: json-schema/openf1-cardata-schema.json
slug: openf1-cardata
source_filename: openf1-cardata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/openf1/json-schema/openf1-cardata-schema.json\",\n  \"title\": \"OpenF1 Car Telemetry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meeting_key\": {\"type\": \"integer\"},\n    \"session_key\": {\"type\": \"integer\"},\n    \"driver_number\": {\"type\": \"integer\"},\n    \"date\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"rpm\": {\"type\": \"integer\"},\n    \"speed\": {\"type\": \"integer\"},\n    \"n_gear\": {\"type\": \"integer\"},\n    \"throttle\": {\"type\": \"integer\"},\n    \"brake\": {\"type\": \"integer\"},\n    \"drs\": {\"type\": \"integer\"}\n  },\n  \"required\": [\"session_key\", \"driver_number\", \"date\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openf1/refs/heads/main/json-schema/openf1-cardata-schema.json
tags:
- Formula 1
- Motorsport
- Telemetry
- Real-Time
- Sports
title: OpenF1 Car Telemetry
---
