---
description: part of the trip covered by the travel class restriction (ALL_SEGMENTS if ommited)
layout: schema
name: Coverage
properties_list: []
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-coverage-schema.json
slug: flight-offers-search-coverage
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Coverage\",\n  \"description\": \"part of the trip covered by the travel class restriction (ALL_SEGMENTS if ommited)\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"MOST_SEGMENTS\",\n    \"AT_LEAST_ONE_SEGMENT\",\n    \"ALL_SEGMENTS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-coverage-schema.json
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
title: Coverage
---
