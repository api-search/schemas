---
description: Error_400 schema
layout: schema
name: Error_400
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-error_400-schema.json
slug: transfer-booking-error_400
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-error_400-schema.json\",\n  \"title\": \"Error_400\",\n  \"description\": \"Error_400 schema\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ],\n  \"example\": {\n    \"errors\": [\n      {\n        \"status\": 400,\n        \"code\": 4926,\n        \"title\": \"INVALID DATA RECEIVED\",\n        \"detail\": \"Transfer type is not valid\",\n        \"source\": {\n          \"parameter\": \"transferType\"\n        }\n      }\n    ]\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-error_400-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Error_400
---
