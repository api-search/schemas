---
description: Hotel Content
layout: schema
name: Hotel
properties_list:
- description: Amadeus Property Code (8 chars)
  name: hotelId
  type: string
- description: Brand (RT...) or Merchant (AD...) (Amadeus 2 chars Code)
  name: chainCode
  type: string
- description: Brand (RT...) (Amadeus 2 chars Code). Small Properties distributed by Merchants may not have a Brand. Example - AD (Value Hotels) is the Provider/Merchant, and RT (Accor) is the Brand of the Property
  name: brandCode
  type: string
- description: Unique Property identifier of the physical hotel. One physical hotel can be represented by different Providers, each one having its own `hotelID`. This attribute allows a client application to group t
  name: dupeId
  type: string
- description: Hotel Name
  name: name
  type: string
- description: 'Warning: The IATA city code associated to the hotel (not necessary the real Hotel City)'
  name: cityCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotel-schema.json
slug: hotel-search-hotel
source_filename: hotel-search-hotel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Hotel\",\n  \"description\": \"Hotel Content\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotelId\": {\n      \"type\": \"string\",\n      \"description\": \"Amadeus Property Code (8 chars)\"\n    },\n    \"chainCode\": {\n      \"type\": \"string\",\n      \"description\": \"Brand (RT...) or Merchant (AD...) (Amadeus 2 chars Code)\"\n    },\n    \"brandCode\": {\n      \"type\": \"string\",\n      \"description\": \"Brand (RT...) (Amadeus 2 chars Code). Small Properties distributed by Merchants may not have a Brand.\\nExample - AD (Value Hotels) is the Provider/Merchant, and RT (Accor) is the Brand of the Property\"\n    },\n    \"dupeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Property identifier of the physical hotel.\\nOne physical hotel can be represented by different Providers, each one having its own `hotelID`.\\nThis attribute allows a client application\
  \ to group together hotels that are actually the same.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel Name\"\n    },\n    \"cityCode\": {\n      \"type\": \"string\",\n      \"description\": \"Warning: The IATA city code associated to the hotel (not necessary the real Hotel City)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotel-schema.json
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
title: Hotel
---
