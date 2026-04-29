---
description: guests schema
layout: schema
name: guests
properties_list:
- description: number of adult guests (1-9) per room
  name: adults
  type: integer
- description: Comma separated list of ages of each child at the time of check-out from the hotel. If several children have the same age, the ages will be repeated.
  name: childAges
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-guests-schema.json
slug: hotel-booking-guests
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-guests-schema.json\",\n  \"title\": \"guests\",\n  \"description\": \"guests schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 9,\n      \"example\": 2,\n      \"description\": \"number of adult guests (1-9) per room\"\n    },\n    \"childAges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"minimum\": 0,\n        \"maximum\": 20\n      },\n      \"description\": \"Comma separated list of ages of each child at the time of check-out from the hotel. If several children have the same age, the ages will be repeated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-guests-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: guests
---
