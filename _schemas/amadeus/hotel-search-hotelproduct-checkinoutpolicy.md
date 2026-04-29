---
description: ''
layout: schema
name: HotelProduct_CheckInOutPolicy
properties_list:
- description: Check-in From time limit in ISO-8601 format [http://www.w3.org/TR/xmlschema-2/#time]
  name: checkIn
  type: string
- description: ''
  name: checkInDescription
  type: object
- description: Check-out Until time limit in ISO-8601 format [http://www.w3.org/TR/xmlschema-2/#time]
  name: checkOut
  type: string
- description: ''
  name: checkOutDescription
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-checkinoutpolicy-schema.json
slug: hotel-search-hotelproduct-checkinoutpolicy
source_filename: hotel-search-hotelproduct-checkinoutpolicy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_CheckInOutPolicy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkIn\": {\n      \"type\": \"string\",\n      \"description\": \"Check-in From time limit in ISO-8601 format [http://www.w3.org/TR/xmlschema-2/#time]\"\n    },\n    \"checkInDescription\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    },\n    \"checkOut\": {\n      \"type\": \"string\",\n      \"description\": \"Check-out Until time limit in ISO-8601 format [http://www.w3.org/TR/xmlschema-2/#time]\"\n    },\n    \"checkOutDescription\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-checkinoutpolicy-schema.json
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
title: HotelProduct_CheckInOutPolicy
---
