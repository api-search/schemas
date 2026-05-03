---
description: ''
layout: schema
name: OpenF1 Lap
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
  name: lap_number
  type: integer
- description: ''
  name: date_start
  type: string
- description: ''
  name: duration_sector_1
  type: number
- description: ''
  name: duration_sector_2
  type: number
- description: ''
  name: duration_sector_3
  type: number
- description: ''
  name: i1_speed
  type: integer
- description: ''
  name: i2_speed
  type: integer
- description: ''
  name: st_speed
  type: integer
- description: ''
  name: is_pit_out_lap
  type: boolean
- description: ''
  name: lap_duration
  type: number
provider_name: OpenF1
provider_slug: openf1
schema_file: json-schema/openf1-lap-schema.json
slug: openf1-lap
source_filename: openf1-lap-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/openf1/json-schema/openf1-lap-schema.json\",\n  \"title\": \"OpenF1 Lap\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meeting_key\": {\"type\": \"integer\"},\n    \"session_key\": {\"type\": \"integer\"},\n    \"driver_number\": {\"type\": \"integer\"},\n    \"lap_number\": {\"type\": \"integer\"},\n    \"date_start\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"duration_sector_1\": {\"type\": \"number\"},\n    \"duration_sector_2\": {\"type\": \"number\"},\n    \"duration_sector_3\": {\"type\": \"number\"},\n    \"i1_speed\": {\"type\": \"integer\"},\n    \"i2_speed\": {\"type\": \"integer\"},\n    \"st_speed\": {\"type\": \"integer\"},\n    \"is_pit_out_lap\": {\"type\": \"boolean\"},\n    \"lap_duration\": {\"type\": \"number\"}\n  },\n  \"required\": [\"session_key\", \"driver_number\", \"lap_number\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openf1/refs/heads/main/json-schema/openf1-lap-schema.json
tags:
- Formula 1
- Motorsport
- Telemetry
- Real-Time
- Sports
title: OpenF1 Lap
---
