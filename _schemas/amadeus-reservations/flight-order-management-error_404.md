---
description: Error_404 schema
layout: schema
name: Error_404
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-error_404-schema.json
slug: flight-order-management-error_404
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-error_404-schema.json\",\n  \"title\": \"Error_404\",\n  \"description\": \"Error_404 schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 404,\n        \"code\": 1797,\n        \"title\": \"NOT FOUND\",\n        \"detail\": \"no response found for this query parameter\",\n        \"source\": {\n          \"parameter\": \"airport\"\n        }\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-error_404-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Error_404
---
