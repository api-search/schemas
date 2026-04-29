---
description: Characteristics for a group of seat, such as Distance from one seat to the another in front or behind it or width space
layout: schema
name: Amenity_Seat
properties_list:
- description: Space between 2 seats
  name: legSpace
  type: integer
- description: ''
  name: spaceUnit
  type: string
- description: Flatness of a seat
  name: tilt
  type: string
- description: ''
  name: amenityType
  type: string
- description: list of media associated to the seat (rich content)
  name: medias
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-amenity-seat-schema.json
slug: seatmap-display-amenity-seat
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Amenity_Seat\",\n  \"description\": \"Characteristics for a group of seat, such as Distance from one seat to the another in front or behind it or width space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legSpace\": {\n      \"type\": \"integer\",\n      \"description\": \"Space between 2 seats\"\n    },\n    \"spaceUnit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INCHES\",\n        \"CENTIMENTERS\"\n      ]\n    },\n    \"tilt\": {\n      \"type\": \"string\",\n      \"description\": \"Flatness of a seat\",\n      \"enum\": [\n        \"FULL_FLAT\",\n        \"ANGLE_FLAT\",\n        \"NORMAL\"\n      ]\n    },\n    \"amenityType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SEAT\"\n      ]\n    },\n    \"medias\": {\n      \"type\": \"array\",\n      \"description\": \"list of media associated to the seat (rich content)\",\n      \"items\": {\n   \
  \     \"$ref\": \"#/definitions/Amenity_Media\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-amenity-seat-schema.json
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
title: Amenity_Seat
---
