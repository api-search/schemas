---
description: Hotel product
layout: schema
name: hotelData
properties_list:
- description: Confirmation number
  name: confirmationNumber
  type: string
- description: heck-in date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is today date (no dates in the past).
  name: checkInDate
  type: string
- description: check-out date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is checkInDate+1.
  name: checkOutDate
  type: string
- description: number of rooms (1-9)
  name: roomQuantity
  type: integer
- description: ''
  name: contact
  type: object
- description: ''
  name: address
  type: object
- description: amenities (list)
  name: amenities
  type: array
- description: Hotel Name
  name: name
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: policies
  type: object
- description: ''
  name: guests
  type: object
- description: ''
  name: room
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-hoteldata-schema.json
slug: trip-parser-hoteldata
source_filename: trip-parser-hoteldata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"hotelData\",\n  \"description\": \"\\t\\nHotel product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Confirmation number\"\n    },\n    \"checkInDate\": {\n      \"type\": \"string\",\n      \"description\": \"heck-in date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is today date (no dates in the past).\"\n    },\n    \"checkOutDate\": {\n      \"type\": \"string\",\n      \"description\": \"check-out date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is checkInDate+1.\"\n    },\n    \"roomQuantity\": {\n      \"type\": \"integer\",\n      \"description\": \"number of rooms (1-9)\"\n    },\n    \"contact\": {\n      \"$ref\": \"#/definitions/contactHotel\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/address\"\n    },\n    \"amenities\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"amenities (list)\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel Name\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/description\"\n    },\n    \"policies\": {\n      \"$ref\": \"#/definitions/policies\"\n    },\n    \"guests\": {\n      \"$ref\": \"#/definitions/guests\"\n    },\n    \"room\": {\n      \"$ref\": \"#/definitions/room\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-hoteldata-schema.json
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
title: hotelData
---
