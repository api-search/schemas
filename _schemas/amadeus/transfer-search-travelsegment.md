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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-travelsegment-schema.json
slug: transfer-search-travelsegment
source_filename: transfer-search-travelsegment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TravelSegment\",\n  \"description\": \"A segment of an itinerary used by a traveler between 2 locations at a given date and time using a particular transportation type FLIGHT or TRAIN\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transportationType\": {\n      \"$ref\": \"#/definitions/TransportationType\"\n    },\n    \"transportationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The flight number or train number, e.g. AF380\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/definitions/TravelSegmentLocation\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/TravelSegmentLocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-travelsegment-schema.json
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
title: TravelSegment
---
