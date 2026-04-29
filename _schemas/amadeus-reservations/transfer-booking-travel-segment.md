---
description: A segment of an itinerary used by a traveler between 2 locations at a given date and time using a particular transportation type FLIGHT or TRAIN
layout: schema
name: TravelSegment
properties_list:
- description: ''
  name: transportationType
  type: object
- description: The flight number or train number, e.g. AF380
  name: transportationNumber
  type: string
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-travel-segment-schema.json
slug: transfer-booking-travel-segment
source_filename: transfer-booking-travel-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-travel-segment-schema.json\",\n  \"title\": \"TravelSegment\",\n  \"description\": \"A segment of an itinerary used by a traveler between 2 locations at a given date and time using a particular transportation type FLIGHT or TRAIN\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transportationType\": {\n      \"$ref\": \"#/definitions/TransportationType\"\n    },\n    \"transportationNumber\": {\n      \"type\": \"string\",\n      \"example\": \"AF380\",\n      \"description\": \"The flight number or train number, e.g. AF380\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/definitions/TravelSegmentLocation\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/TravelSegmentLocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-travel-segment-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TravelSegment
---
