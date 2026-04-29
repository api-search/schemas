---
description: The estimated rate code family of the offer. Grouping various rate plan codes that belongs to the same family and indicates the type of the rate
layout: schema
name: HotelProduct_RateFamily
properties_list:
- description: The estimated rate family (PRO,FAM,GOV)
  name: code
  type: string
- description: The type of the rate (public=P, negotiated=N, conditional=C)
  name: type
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-ratefamily-schema.json
slug: hotel-search-hotelproduct-ratefamily
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_RateFamily\",\n  \"description\": \"The estimated rate code family of the offer. Grouping various rate plan codes that belongs to the same family and indicates the type of the rate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The estimated rate family (PRO,FAM,GOV)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the rate (public=P, negotiated=N, conditional=C)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-ratefamily-schema.json
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
title: HotelProduct_RateFamily
---
