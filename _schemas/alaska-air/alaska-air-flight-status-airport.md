---
description: Airport departure or arrival information
layout: schema
name: Airport
properties_list:
- description: IATA airport code
  name: airportCode
  type: string
- description: Full airport name
  name: airportName
  type: string
- description: Scheduled departure time with timezone
  name: scheduledDeparture
  type: string
- description: Estimated departure time with timezone
  name: estimatedDeparture
  type: string
- description: Scheduled arrival time with timezone
  name: scheduledArrival
  type: string
- description: Estimated arrival time with timezone
  name: estimatedArrival
  type: string
- description: Gate assignment
  name: gate
  type: string
- description: Terminal designation
  name: terminal
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-status-airport-schema.json
slug: alaska-air-flight-status-airport
source_filename: alaska-air-flight-status-airport-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-airport-schema.json\",\n  \"title\": \"Airport\",\n  \"description\": \"Airport departure or arrival information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"airportCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA airport code\",\n      \"example\": \"SEA\"\n    },\n    \"airportName\": {\n      \"type\": \"string\",\n      \"description\": \"Full airport name\",\n      \"example\": \"Seattle-Tacoma International Airport\"\n    },\n    \"scheduledDeparture\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled departure time with timezone\",\n      \"example\": \"2026-04-19T08:30:00-07:00\"\n    },\n    \"estimatedDeparture\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Estimated departure time with timezone\",\n      \"example\": \"2026-04-19T08:30:00-07:00\"\n    },\n    \"scheduledArrival\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled arrival time with timezone\",\n      \"example\": \"2026-04-19T11:05:00-07:00\"\n    },\n    \"estimatedArrival\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated arrival time with timezone\",\n      \"example\": \"2026-04-19T11:05:00-07:00\"\n    },\n    \"gate\": {\n      \"type\": \"string\",\n      \"description\": \"Gate assignment\",\n      \"example\": \"D6\"\n    },\n    \"terminal\": {\n      \"type\": \"string\",\n      \"description\": \"Terminal designation\",\n      \"example\": \"S\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-airport-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Airport
---
