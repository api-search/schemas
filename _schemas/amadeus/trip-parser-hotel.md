---
description: ''
layout: schema
name: hotel
properties_list:
- description: ''
  name: hotel
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-hotel-schema.json
slug: trip-parser-hotel
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"hotel\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotel\": {\n      \"$ref\": \"#/definitions/hotelData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-hotel-schema.json
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
title: hotel
---
