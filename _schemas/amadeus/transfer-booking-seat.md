---
description: ''
layout: schema
name: Seat
properties_list:
- description: seat capacity
  name: count
  type: integer
- description: seat row
  name: row
  type: string
- description: seat size
  name: size
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-seat-schema.json
slug: transfer-booking-seat
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Seat\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"seat capacity\"\n    },\n    \"row\": {\n      \"type\": \"string\",\n      \"description\": \"seat row\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"seat size\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-seat-schema.json
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
title: Seat
---
