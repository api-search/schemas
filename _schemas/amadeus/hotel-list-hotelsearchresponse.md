---
description: ''
layout: schema
name: HotelSearchResponse
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-list-hotelsearchresponse-schema.json
slug: hotel-list-hotelsearchresponse
source_filename: hotel-list-hotelsearchresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelSearchResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Hotel\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Meta\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-list-hotelsearchresponse-schema.json
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
title: HotelSearchResponse
---
