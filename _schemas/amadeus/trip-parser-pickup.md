---
description: Pick-up location and time of the rented vehicle.
layout: schema
name: pickup
properties_list:
- description: local date and time compliant with ISO8601.
  name: localDateTime
  type: string
- description: ''
  name: location
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-pickup-schema.json
slug: trip-parser-pickup
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"pickup\",\n  \"description\": \"\\t\\nPick-up location and time of the rented vehicle.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"localDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"local date and time compliant with ISO8601.\"\n    },\n    \"location\": {\n      \"$ref\": \"#/definitions/location\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-pickup-schema.json
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
title: pickup
---
