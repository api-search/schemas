---
description: ''
layout: schema
name: seats
properties_list:
- description: Seat number corresponding to the concatenation of the seatmap row and the column information, for example 12B'
  name: number
  type: string
- description: Cabin code associated to the seat
  name: cabin
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-seats-schema.json
slug: trip-parser-seats
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"seats\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Seat number corresponding to the concatenation of the seatmap row and the column information, for example 12B'\"\n    },\n    \"cabin\": {\n      \"type\": \"string\",\n      \"description\": \"Cabin code associated to the seat\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-seats-schema.json
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
title: seats
---
