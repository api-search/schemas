---
description: Error_400 schema
layout: schema
name: Error_400
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-error_400-schema.json
slug: flight-offers-price-error_400
source_filename: flight-offers-price-error_400-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-error_400-schema.json\",\n  \"title\": \"Error_400\",\n  \"description\": \"Error_400 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 400,\n        \"code\": 477,\n        \"title\": \"INVALID FORMAT\",\n        \"detail\": \"invalid query parameter format\",\n        \"source\": {\n          \"parameter\": \"airport\",\n          \"example\": \"CDG\"\n        }\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-error_400-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Error_400
---
