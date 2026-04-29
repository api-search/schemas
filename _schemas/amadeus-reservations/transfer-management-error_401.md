---
description: Error_401 schema
layout: schema
name: Error_401
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-management-error_401-schema.json
slug: transfer-management-error_401
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-management-error_401-schema.json\",\n  \"title\": \"Error_401\",\n  \"description\": \"Error_401 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 401,\n        \"code\": 20,\n        \"title\": \"RESTRICTED\",\n        \"detail\": \"Query unauthorized\"\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-management-error_401-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Error_401
---
