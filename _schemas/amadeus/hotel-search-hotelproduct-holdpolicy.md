---
description: the hold policy
layout: schema
name: HotelProduct_HoldPolicy
properties_list:
- description: 'The date and time of the deadline in ISO 8601[https://www.w3.org/TR/NOTE-datetime]. Example: 2010-08-14T13:00:00 Please note that this value is expressed in the hotels local time zone'
  name: deadline
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-holdpolicy-schema.json
slug: hotel-search-hotelproduct-holdpolicy
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_HoldPolicy\",\n  \"description\": \"the hold policy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deadline\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the deadline in ISO 8601[https://www.w3.org/TR/NOTE-datetime]. \\n Example: 2010-08-14T13:00:00\\n Please note that this value is expressed in the hotels local time zone\"\n    }\n  },\n  \"required\": [\n    \"deadline\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-holdpolicy-schema.json
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
title: HotelProduct_HoldPolicy
---
