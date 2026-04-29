---
description: Seat schema
layout: schema
name: Seat
properties_list:
- description: Cabin of the seat.
  name: cabin
  type: string
- description: Concatenation of the row id and the column id, for example 12B
  name: number
  type: string
- description: 'List of seat characteristics (the characteristic''s names can be retrieved in the seat characteristic dictionary) Possible values are part of: IATA code: Most of the codes are defined by IATA Standard/'
  name: characteristicsCodes
  type: array
- description: Traveler's information and price
  name: travelerPricing
  type: array
- description: ''
  name: coordinates
  type: object
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-seat-schema.json
slug: seat-map-display-seat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seat-schema.json\",\n  \"title\": \"Seat\",\n  \"description\": \"Seat schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cabin\": {\n      \"description\": \"Cabin of the seat.\",\n      \"type\": \"string\",\n      \"example\": \"ECO\"\n    },\n    \"number\": {\n      \"description\": \"Concatenation of the row id and the column id, for example 12B\",\n      \"type\": \"string\",\n      \"example\": \"12B\"\n    },\n    \"characteristicsCodes\": {\n      \"description\": \"List of seat characteristics (the characteristic's names can be retrieved in the seat characteristic dictionary) Possible values are part of:\\n\\n  IATA code: Most of the codes are defined by IATA Standard/IATA Code list 9825\\n\\n  Amadeus Code: defined as extension, example MV=row with movie screen\\\
  n\\n  Seat map display Code: API specific codes, example 1A_AQC_PREMIUM_SEAT=premium seat\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"travelerPricing\": {\n      \"description\": \"Traveler's information and price\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/SeatmapTravelerPricing\"\n      }\n    },\n    \"coordinates\": {\n      \"$ref\": \"#/definitions/Coordinates\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seat-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Seat
---
