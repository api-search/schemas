---
description: Seat schema
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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-seat-schema.json
slug: transfer-booking-seat
source_filename: transfer-booking-seat-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-seat-schema.json\",\n  \"title\": \"Seat\",\n  \"description\": \"Seat schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"seat capacity\",\n      \"example\": 3\n    },\n    \"row\": {\n      \"type\": \"string\",\n      \"description\": \"seat row\",\n      \"example\": \"front\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"seat size\",\n      \"example\": \"XL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-seat-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Seat
---
