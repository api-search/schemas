---
description: ''
layout: schema
name: OpenF1 Driver
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
  name: broadcast_name
  type: string
- description: ''
  name: full_name
  type: string
- description: ''
  name: name_acronym
  type: string
- description: ''
  name: team_name
  type: string
- description: ''
  name: team_colour
  type: string
- description: ''
  name: first_name
  type: string
- description: ''
  name: last_name
  type: string
- description: ''
  name: headshot_url
  type: string
- description: ''
  name: country_code
  type: string
provider_name: OpenF1
provider_slug: openf1
schema_file: json-schema/openf1-driver-schema.json
slug: openf1-driver
source_filename: openf1-driver-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/openf1/json-schema/openf1-driver-schema.json\",\n  \"title\": \"OpenF1 Driver\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meeting_key\": {\"type\": \"integer\"},\n    \"session_key\": {\"type\": \"integer\"},\n    \"driver_number\": {\"type\": \"integer\"},\n    \"broadcast_name\": {\"type\": \"string\"},\n    \"full_name\": {\"type\": \"string\"},\n    \"name_acronym\": {\"type\": \"string\"},\n    \"team_name\": {\"type\": \"string\"},\n    \"team_colour\": {\"type\": \"string\"},\n    \"first_name\": {\"type\": \"string\"},\n    \"last_name\": {\"type\": \"string\"},\n    \"headshot_url\": {\"type\": \"string\", \"format\": \"uri\"},\n    \"country_code\": {\"type\": \"string\"}\n  },\n  \"required\": [\"session_key\", \"driver_number\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openf1/refs/heads/main/json-schema/openf1-driver-schema.json
tags:
- Formula 1
- Motorsport
- Telemetry
- Real-Time
- Sports
title: OpenF1 Driver
---
