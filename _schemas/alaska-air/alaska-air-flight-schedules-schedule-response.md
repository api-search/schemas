---
description: Flight schedule query response
layout: schema
name: ScheduleResponse
properties_list:
- description: Origin airport IATA code
  name: origin
  type: string
- description: Destination airport IATA code
  name: destination
  type: string
- description: Query departure date
  name: departureDate
  type: string
- description: List of scheduled flights
  name: schedules
  type: array
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-schedules-schedule-response-schema.json
slug: alaska-air-flight-schedules-schedule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-schedule-response-schema.json\",\n  \"title\": \"ScheduleResponse\",\n  \"description\": \"Flight schedule query response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\",\n      \"example\": \"LAX\"\n    },\n    \"departureDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Query departure date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"schedules\": {\n      \"type\": \"array\",\n      \"description\": \"List of scheduled flights\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Schedule\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-schedule-response-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: ScheduleResponse
---
