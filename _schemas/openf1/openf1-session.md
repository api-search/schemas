---
description: ''
layout: schema
name: OpenF1 Session
properties_list:
- description: ''
  name: session_key
  type: integer
- description: ''
  name: session_name
  type: string
- description: ''
  name: session_type
  type: string
- description: ''
  name: date_start
  type: string
- description: ''
  name: date_end
  type: string
- description: ''
  name: meeting_key
  type: integer
- description: ''
  name: circuit_key
  type: integer
- description: ''
  name: circuit_short_name
  type: string
- description: ''
  name: country_key
  type: integer
- description: ''
  name: country_code
  type: string
- description: ''
  name: country_name
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: gmt_offset
  type: string
- description: ''
  name: year
  type: integer
- description: ''
  name: is_cancelled
  type: boolean
provider_name: OpenF1
provider_slug: openf1
schema_file: json-schema/openf1-session-schema.json
slug: openf1-session
source_filename: openf1-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/openf1/json-schema/openf1-session-schema.json\",\n  \"title\": \"OpenF1 Session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"session_key\": {\"type\": \"integer\"},\n    \"session_name\": {\"type\": \"string\"},\n    \"session_type\": {\"type\": \"string\"},\n    \"date_start\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"date_end\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"meeting_key\": {\"type\": \"integer\"},\n    \"circuit_key\": {\"type\": \"integer\"},\n    \"circuit_short_name\": {\"type\": \"string\"},\n    \"country_key\": {\"type\": \"integer\"},\n    \"country_code\": {\"type\": \"string\"},\n    \"country_name\": {\"type\": \"string\"},\n    \"location\": {\"type\": \"string\"},\n    \"gmt_offset\": {\"type\": \"string\"},\n    \"year\": {\"type\": \"integer\"},\n    \"is_cancelled\": {\"type\": \"boolean\"\
  }\n  },\n  \"required\": [\"session_key\", \"meeting_key\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openf1/refs/heads/main/json-schema/openf1-session-schema.json
tags:
- Formula 1
- Motorsport
- Telemetry
- Real-Time
- Sports
title: OpenF1 Session
---
