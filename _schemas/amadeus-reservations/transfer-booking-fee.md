---
description: single fee information
layout: schema
name: Fee
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-fee-schema.json
slug: transfer-booking-fee
source_filename: transfer-booking-fee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-fee-schema.json\",\n  \"title\": \"Fee\",\n  \"description\": \"single fee information\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/PointsAndCash\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"currencyCode\": {\n          \"type\": \"string\",\n          \"example\": \"USD\"\n        },\n        \"indicator\": {\n          \"type\": \"string\",\n          \"description\": \"fee category e.g. \\\"AIRPORT\\\", \\\"CREDITCARD\\\" ,\\\"CANCELLATION\\\"\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-fee-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Fee
---
