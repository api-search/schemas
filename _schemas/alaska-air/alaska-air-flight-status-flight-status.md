---
description: Real-time status for an Alaska Airlines flight
layout: schema
name: FlightStatus
properties_list:
- description: Flight number including carrier code
  name: flightNumber
  type: string
- description: Flight operating date
  name: flightDate
  type: string
- description: Operating carrier code
  name: carrier
  type: string
- description: Flight status description
  name: status
  type: string
- description: Delay in minutes (0 if on time)
  name: delayMinutes
  type: integer
- description: Reason for delay if applicable
  name: delayReason
  type: string
- description: ''
  name: origin
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: aircraft
  type: object
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-status-flight-status-schema.json
slug: alaska-air-flight-status-flight-status
source_filename: alaska-air-flight-status-flight-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-flight-status-schema.json\",\n  \"title\": \"FlightStatus\",\n  \"description\": \"Real-time status for an Alaska Airlines flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Flight number including carrier code\",\n      \"example\": \"AS123\"\n    },\n    \"flightDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Flight operating date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Operating carrier code\",\n      \"enum\": [\n        \"AS\",\n        \"QX\"\n      ],\n      \"example\": \"AS\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Flight status\
  \ description\",\n      \"enum\": [\n        \"On Time\",\n        \"Delayed\",\n        \"Cancelled\",\n        \"Departed\",\n        \"Arrived\",\n        \"Diverted\"\n      ],\n      \"example\": \"On Time\"\n    },\n    \"delayMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay in minutes (0 if on time)\",\n      \"example\": 0\n    },\n    \"delayReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for delay if applicable\",\n      \"example\": \"Late arriving aircraft\"\n    },\n    \"origin\": {\n      \"$ref\": \"#/components/schemas/Airport\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/components/schemas/Airport\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/components/schemas/Aircraft\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-flight-status-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: FlightStatus
---
