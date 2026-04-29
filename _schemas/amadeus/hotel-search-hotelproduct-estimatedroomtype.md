---
description: estimated room category, bed type and number of beds in the room. This information has been parsed from the room description, and is thus only provided for informational purposes
layout: schema
name: HotelProduct_EstimatedRoomType
properties_list:
- description: Category code
  name: category
  type: string
- description: Number of beds in the room (1-9)
  name: beds
  type: integer
- description: Type of the bed
  name: bedType
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-estimatedroomtype-schema.json
slug: hotel-search-hotelproduct-estimatedroomtype
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_EstimatedRoomType\",\n  \"description\": \"estimated room category, bed type and number of beds in the room. This information has been parsed from the room description, and is thus only provided for informational purposes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category code\"\n    },\n    \"beds\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of beds in the room (1-9)\"\n    },\n    \"bedType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the bed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-estimatedroomtype-schema.json
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
title: HotelProduct_EstimatedRoomType
---
