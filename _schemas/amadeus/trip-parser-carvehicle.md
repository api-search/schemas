---
description: ''
layout: schema
name: carVehicle
properties_list:
- description: Association of car rental industry systems standards
  name: acrissCode
  type: string
- description: Car model name
  name: carModel
  type: string
- description: Number of doors
  name: doors
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-carvehicle-schema.json
slug: trip-parser-carvehicle
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"carVehicle\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acrissCode\": {\n      \"type\": \"string\",\n      \"description\": \"Association of car rental industry systems standards\"\n    },\n    \"carModel\": {\n      \"type\": \"string\",\n      \"description\": \"Car model name\"\n    },\n    \"doors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of doors\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-carvehicle-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: carVehicle
---
