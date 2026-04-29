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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-amenity_-seat-schema.json
slug: seat-map-display-amenity_-seat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-amenity_-seat-schema.json\",\n  \"title\": \"Amenity_Seat\",\n  \"description\": \"Characteristics for a group of seat, such as Distance from one seat to the another in front or behind it or width space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legSpace\": {\n      \"description\": \"Space between 2 seats\",\n      \"type\": \"integer\",\n      \"example\": 33\n    },\n    \"spaceUnit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INCHES\",\n        \"CENTIMENTERS\"\n      ]\n    },\n    \"tilt\": {\n      \"description\": \"Flatness of a seat\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"FULL_FLAT\",\n        \"ANGLE_FLAT\",\n        \"NORMAL\"\n      ]\n    },\n    \"amenityType\": {\n      \"type\": \"string\",\n      \"enum\": [\n  \
  \      \"SEAT\"\n      ]\n    },\n    \"medias\": {\n      \"description\": \"list of media associated to the seat (rich content)\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Amenity_Media\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-amenity_-seat-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Amenity_Seat
---
