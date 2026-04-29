---
description: Departure or arrival information
layout: schema
name: arrivalAir
properties_list:
- description: IATA Airport code
  name: iataCode
  type: string
- description: Terminal name / number
  name: terminal
  type: string
- description: Local schedule dateTime of the departure or arrival. Conversion of dateTime in local date time.
  name: localDateTime
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-arrivalair-schema.json
slug: trip-parser-arrivalair
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"arrivalAir\",\n  \"description\": \"Departure or arrival information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA Airport code\"\n    },\n    \"terminal\": {\n      \"type\": \"string\",\n      \"description\": \"Terminal name / number\"\n    },\n    \"localDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Local schedule dateTime of the departure or arrival. Conversion of dateTime in local date time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-arrivalair-schema.json
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
title: arrivalAir
---
