---
description: ''
layout: schema
name: HotelProduct_Guests
properties_list:
- description: number of adult guests (1-9) per room
  name: adults
  type: integer
- description: Comma separated list of ages of each child at the time of check-out from the hotel. If several children have the same age, the ages will be repeated.
  name: childAges
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-guests-schema.json
slug: hotel-search-hotelproduct-guests
source_filename: hotel-search-hotelproduct-guests-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_Guests\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adults\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"number of adult guests (1-9) per room\"\n    },\n    \"childAges\": {\n      \"type\": \"array\",\n      \"description\": \"Comma separated list of ages of each child at the time of check-out from the hotel. If several children have the same age, the ages will be repeated.\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-guests-schema.json
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
title: HotelProduct_Guests
---
