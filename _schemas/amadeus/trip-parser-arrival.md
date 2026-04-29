---
description: Description of a particular point or place in physical space
layout: schema
name: arrival
properties_list:
- description: Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)
  name: subtype
  type: string
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: IATA location code
  name: iataCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-arrival-schema.json
slug: trip-parser-arrival
source_filename: trip-parser-arrival-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"arrival\",\n  \"description\": \"\\t\\nDescription of a particular point or place in physical space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Label associated to the location (e.g. Eiffel Tower, Madison Square)\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA location code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-arrival-schema.json
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
title: arrival
---
