---
description: ''
layout: schema
name: room
properties_list:
- description: Room type code, 3 character identifier of the room. The first character identifies the room type category. The second numeric character identifies the number of beds. The third character identifies th
  name: type
  type: string
- description: ''
  name: typeEstimated
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-room-schema.json
slug: trip-parser-room
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"room\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Room type code, 3 character identifier of the room. The first character identifies the room type category. The second numeric character identifies the number of beds. The third character identifies the bed type. There is a special case where ROH is returned, this value stands for Run Of House.\"\n    },\n    \"typeEstimated\": {\n      \"$ref\": \"#/definitions/typeEstimated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-room-schema.json
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
title: room
---
