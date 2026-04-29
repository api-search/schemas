---
description: A scheduled flight between two airports
layout: schema
name: Schedule
properties_list:
- description: Alaska Airlines flight number
  name: flightNumber
  type: string
- description: Operating carrier code
  name: carrier
  type: string
- description: Scheduled departure time (HH:MM local)
  name: departureTime
  type: string
- description: Scheduled arrival time (HH:MM local)
  name: arrivalTime
  type: string
- description: Flight duration in minutes
  name: duration
  type: integer
- description: Aircraft type/model
  name: aircraft
  type: string
- description: Days of week this flight operates
  name: operatingDays
  type: array
- description: Number of intermediate stops
  name: stops
  type: integer
- description: Available cabin class
  name: cabin
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-schedules-schedule-schema.json
slug: alaska-air-flight-schedules-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-schedule-schema.json\",\n  \"title\": \"Schedule\",\n  \"description\": \"A scheduled flight between two airports\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Alaska Airlines flight number\",\n      \"example\": \"AS123\"\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Operating carrier code\",\n      \"enum\": [\n        \"AS\",\n        \"QX\"\n      ],\n      \"example\": \"AS\"\n    },\n    \"departureTime\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled departure time (HH:MM local)\",\n      \"example\": \"08:30\"\n    },\n    \"arrivalTime\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled arrival time (HH:MM local)\"\
  ,\n      \"example\": \"11:05\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Flight duration in minutes\",\n      \"example\": 155\n    },\n    \"aircraft\": {\n      \"type\": \"string\",\n      \"description\": \"Aircraft type/model\",\n      \"example\": \"Boeing 737-900ER\"\n    },\n    \"operatingDays\": {\n      \"type\": \"array\",\n      \"description\": \"Days of week this flight operates\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Monday\",\n        \"Wednesday\",\n        \"Friday\"\n      ]\n    },\n    \"stops\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of intermediate stops\",\n      \"example\": 0\n    },\n    \"cabin\": {\n      \"type\": \"string\",\n      \"description\": \"Available cabin class\",\n      \"enum\": [\n        \"First\",\n        \"Premium Class\",\n        \"Economy\"\n      ],\n      \"example\": \"Economy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-schedule-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Schedule
---
