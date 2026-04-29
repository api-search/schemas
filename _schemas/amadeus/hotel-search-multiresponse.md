---
description: ''
layout: schema
name: MultiResponse
properties_list:
- description: ''
  name: data
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-multiresponse-schema.json
slug: hotel-search-multiresponse
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MultiResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/definitions/HotelOffers\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-multiresponse-schema.json
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
title: MultiResponse
---
