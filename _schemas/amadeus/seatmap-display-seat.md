---
description: ''
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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-seat-schema.json
slug: seatmap-display-seat
source_filename: seatmap-display-seat-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Seat\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cabin\": {\n      \"type\": \"string\",\n      \"description\": \"Cabin of the seat.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Concatenation of the row id and the column id, for example 12B\"\n    },\n    \"characteristicsCodes\": {\n      \"type\": \"array\",\n      \"description\": \"List of seat characteristics (the characteristic's names can be retrieved in the seat characteristic dictionary) Possible values are part of:\\n\\n  IATA code: Most of the codes are defined by IATA Standard/IATA Code list 9825\\n\\n  Amadeus Code: defined as extension, example MV=row with movie screen\\n\\n  Seat map display Code: API specific codes, example 1A_AQC_PREMIUM_SEAT=premium seat\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"travelerPricing\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Traveler's information and price\",\n      \"items\": {\n        \"$ref\": \"#/definitions/SeatmapTravelerPricing\"\n      }\n    },\n    \"coordinates\": {\n      \"$ref\": \"#/definitions/Coordinates\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-seat-schema.json
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
