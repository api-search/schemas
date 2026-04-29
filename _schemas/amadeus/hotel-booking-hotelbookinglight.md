---
description: Booking Details
layout: schema
name: HotelBookingLight
properties_list:
- description: Response Type
  name: type
  type: string
- description: Booking Id
  name: id
  type: string
- description: GDS Confirmation Number. If you call the Provider, this Reference may be asked
  name: providerConfirmationId
  type: string
- description: ''
  name: associatedRecords
  type: array
- description: Retrieve Booking Details
  name: self
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-hotelbookinglight-schema.json
slug: hotel-booking-hotelbookinglight
source_filename: hotel-booking-hotelbookinglight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelBookingLight\",\n  \"description\": \"Booking Details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Response Type\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Booking Id\"\n    },\n    \"providerConfirmationId\": {\n      \"type\": \"string\",\n      \"description\": \"GDS Confirmation Number. If you call the Provider, this Reference may be asked\"\n    },\n    \"associatedRecords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AssociatedRecord\"\n      }\n    },\n    \"self\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Retrieve Booking Details\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"providerConfirmationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-hotelbookinglight-schema.json
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
title: HotelBookingLight
---
