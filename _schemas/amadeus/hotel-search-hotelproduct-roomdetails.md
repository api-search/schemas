---
description: ''
layout: schema
name: HotelProduct_RoomDetails
properties_list:
- description: Room type code, 3 character identifier of the room. The first character identifies the room type category. The second numeric character identifies the number of beds. The third character identifies th
  name: type
  type: string
- description: ''
  name: typeEstimated
  type: object
- description: ''
  name: description
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-roomdetails-schema.json
slug: hotel-search-hotelproduct-roomdetails
source_filename: hotel-search-hotelproduct-roomdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_RoomDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Room type code, 3 character identifier of the room.\\nThe first character identifies the room type category. \\nThe second numeric character identifies the number of beds. \\nThe third character identifies the bed type. \\nThere is a special case where ROH is returned, this value stands for Run Of House.\"\n    },\n    \"typeEstimated\": {\n      \"$ref\": \"#/definitions/HotelProduct_EstimatedRoomType\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-roomdetails-schema.json
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
title: HotelProduct_RoomDetails
---
