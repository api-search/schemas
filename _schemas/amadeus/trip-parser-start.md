---
description: Description of a particular point or place in physical space
layout: schema
name: start
properties_list:
- description: Local Date/Time of the itinerary end in format ISO 8601 (YYYY-MM-DDTHH:MM:SS)
  name: localDateTime
  type: string
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: IATA location code
  name: iataCode
  type: string
- description: ''
  name: address
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-start-schema.json
slug: trip-parser-start
source_filename: trip-parser-start-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"start\",\n  \"description\": \"Description of a particular point or place in physical space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"localDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Local Date/Time of the itinerary end in format ISO 8601 (YYYY-MM-DDTHH:MM:SS)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Label associated to the location (e.g. Eiffel Tower, Madison Square)\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA location code\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-start-schema.json
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
title: start
---
