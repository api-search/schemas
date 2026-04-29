---
description: FlightStatus schema
layout: schema
name: FlightStatus
properties_list:
- description: ''
  name: flightId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: gate
  type: string
- description: ''
  name: delay
  type: integer
provider_name: American Airlines
provider_slug: american-airlines
schema_file: json-schema/runway-developer-api-flight-status-schema.json
slug: runway-developer-api-flight-status
source_filename: runway-developer-api-flight-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-flight-status-schema.json\",\n  \"title\": \"FlightStatus\",\n  \"description\": \"FlightStatus schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"gate\": {\n      \"type\": \"string\"\n    },\n    \"delay\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-flight-status-schema.json
tags:
- Airlines
- Aviation
- Flights
- Travel
- Booking
- Developer Experience
title: FlightStatus
---
