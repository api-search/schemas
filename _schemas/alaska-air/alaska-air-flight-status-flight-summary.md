---
description: Summary flight information for route listing
layout: schema
name: FlightSummary
properties_list:
- description: Flight number
  name: flightNumber
  type: string
- description: Operating carrier code
  name: carrier
  type: string
- description: Flight status
  name: status
  type: string
- description: Scheduled departure time
  name: scheduledDeparture
  type: string
- description: Scheduled arrival time
  name: scheduledArrival
  type: string
- description: Delay in minutes
  name: delayMinutes
  type: integer
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-status-flight-summary-schema.json
slug: alaska-air-flight-status-flight-summary
source_filename: alaska-air-flight-status-flight-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-flight-summary-schema.json\",\n  \"title\": \"FlightSummary\",\n  \"description\": \"Summary flight information for route listing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Flight number\",\n      \"example\": \"AS123\"\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Operating carrier code\",\n      \"example\": \"AS\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Flight status\",\n      \"example\": \"On Time\"\n    },\n    \"scheduledDeparture\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled departure time\",\n      \"example\": \"2026-04-19T08:30:00-07:00\"\n    },\n    \"\
  scheduledArrival\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled arrival time\",\n      \"example\": \"2026-04-19T11:05:00-07:00\"\n    },\n    \"delayMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay in minutes\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-flight-summary-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: FlightSummary
---
