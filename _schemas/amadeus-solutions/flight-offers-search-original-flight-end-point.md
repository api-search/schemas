---
description: departure or arrival information
layout: schema
name: OriginalFlightEndPoint
properties_list:
- description: '[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)'
  name: iataCode
  type: string
- description: terminal name / number
  name: terminal
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-original-flight-end-point-schema.json
slug: flight-offers-search-original-flight-end-point
source_filename: flight-offers-search-original-flight-end-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-original-flight-end-point-schema.json\",\n  \"title\": \"OriginalFlightEndPoint\",\n  \"description\": \"departure or arrival information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\",\n      \"type\": \"string\",\n      \"example\": \"JFK\"\n    },\n    \"terminal\": {\n      \"description\": \"terminal name / number\",\n      \"type\": \"string\",\n      \"example\": \"T2\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-original-flight-end-point-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: OriginalFlightEndPoint
---
