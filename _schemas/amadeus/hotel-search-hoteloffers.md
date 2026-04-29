---
description: ''
layout: schema
name: HotelOffers
properties_list:
- description: the type of the object (hotel-offers)
  name: type
  type: string
- description: ''
  name: available
  type: boolean
- description: ''
  name: self
  type: string
- description: ''
  name: offers
  type: array
- description: ''
  name: hotel
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hoteloffers-schema.json
slug: hotel-search-hoteloffers
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelOffers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the type of the object (hotel-offers)\"\n    },\n    \"available\": {\n      \"type\": \"boolean\"\n    },\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"offers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/HotelOffer\"\n      }\n    },\n    \"hotel\": {\n      \"$ref\": \"#/definitions/Hotel\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hoteloffers-schema.json
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
title: HotelOffers
---
