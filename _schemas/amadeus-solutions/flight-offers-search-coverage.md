---
description: part of the trip covered by the travel class restriction (ALL_SEGMENTS if ommited)
layout: schema
name: Coverage
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-coverage-schema.json
slug: flight-offers-search-coverage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-coverage-schema.json\",\n  \"title\": \"Coverage\",\n  \"description\": \"part of the trip covered by the travel class restriction (ALL_SEGMENTS if ommited)\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"MOST_SEGMENTS\",\n    \"AT_LEAST_ONE_SEGMENT\",\n    \"ALL_SEGMENTS\"\n  ],\n  \"example\": \"MOST_SEGMENTS\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-coverage-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Coverage
---
