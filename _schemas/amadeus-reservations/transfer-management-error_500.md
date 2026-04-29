---
description: Error_500 schema
layout: schema
name: Error_500
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-management-error_500-schema.json
slug: transfer-management-error_500
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-management-error_500-schema.json\",\n  \"title\": \"Error_500\",\n  \"description\": \"Error_500 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 500,\n        \"code\": 141,\n        \"title\": \"SYSTEM ERROR HAS OCCURRED\"\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-management-error_500-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Error_500
---
