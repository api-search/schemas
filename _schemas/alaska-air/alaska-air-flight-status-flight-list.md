---
description: List of flights for a route and date
layout: schema
name: FlightList
properties_list:
- description: Array of flight summaries
  name: flights
  type: array
- description: Origin airport IATA code
  name: originAirport
  type: string
- description: Destination airport IATA code
  name: destinationAirport
  type: string
- description: Flight date
  name: flightDate
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-status-flight-list-schema.json
slug: alaska-air-flight-status-flight-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-flight-list-schema.json\",\n  \"title\": \"FlightList\",\n  \"description\": \"List of flights for a route and date\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flights\": {\n      \"type\": \"array\",\n      \"description\": \"Array of flight summaries\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlightSummary\"\n      }\n    },\n    \"originAirport\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destinationAirport\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\",\n      \"example\": \"LAX\"\n    },\n    \"flightDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Flight date\",\n      \"\
  example\": \"2026-04-19\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-flight-list-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: FlightList
---
