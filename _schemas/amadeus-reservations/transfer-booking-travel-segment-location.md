---
description: The flight or train departure/arrival date&time, location information
layout: schema
name: TravelSegmentLocation
properties_list:
- description: The railway UIC code defined by the worldwide railway organization, e.g. 7400001
  name: uicCode
  type: string
- description: The airport code from IATA table codes, e.g. CDG
  name: iataCode
  type: string
- description: The date and time inspired from ISO 8601 (YYYY-MM-DDTHH:MM:SS) format
  name: localDateTime
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-travel-segment-location-schema.json
slug: transfer-booking-travel-segment-location
source_filename: transfer-booking-travel-segment-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-travel-segment-location-schema.json\",\n  \"title\": \"TravelSegmentLocation\",\n  \"description\": \"The flight or train departure/arrival date&time, location information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uicCode\": {\n      \"type\": \"string\",\n      \"description\": \"The railway UIC code defined by the worldwide railway organization, e.g. 7400001\",\n      \"example\": 7400001\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"The airport code from IATA table codes, e.g. CDG\",\n      \"example\": \"CDG\"\n    },\n    \"localDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time inspired from ISO 8601 (YYYY-MM-DDTHH:MM:SS) format\",\n      \"format\": \"date-time\",\n      \"example\": \"\
  2021-03-27T20:03:00\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-travel-segment-location-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TravelSegmentLocation
---
