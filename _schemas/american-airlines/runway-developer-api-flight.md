---
description: Flight schema
layout: schema
name: Flight
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: flightNumber
  type: string
- description: ''
  name: origin
  type: string
- description: ''
  name: destination
  type: string
- description: ''
  name: departureTime
  type: string
- description: ''
  name: arrivalTime
  type: string
- description: ''
  name: status
  type: string
provider_name: American Airlines
provider_slug: american-airlines
schema_file: json-schema/runway-developer-api-flight-schema.json
slug: runway-developer-api-flight
source_filename: runway-developer-api-flight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-flight-schema.json\",\n  \"title\": \"Flight\",\n  \"description\": \"Flight schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"flightNumber\": {\n      \"type\": \"string\"\n    },\n    \"origin\": {\n      \"type\": \"string\"\n    },\n    \"destination\": {\n      \"type\": \"string\"\n    },\n    \"departureTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"arrivalTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-flight-schema.json
tags:
- Airlines
- Aviation
- Flights
- Travel
- Booking
- Developer Experience
title: Flight
---
