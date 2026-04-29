---
description: single tax information
layout: schema
name: Tax
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-tax-schema.json
slug: transfer-booking-tax
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-tax-schema.json\",\n  \"title\": \"Tax\",\n  \"description\": \"single tax information\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"monetaryAmount\": {\n          \"type\": \"string\",\n          \"example\": \"10.5\"\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"indicator\": {\n          \"type\": \"string\",\n          \"description\": \"Tax category\"\n        },\n        \"natureCode\": {\n          \"type\": \"string\",\n          \"description\": \"Tax code\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\": \"Tax iso country code\"\n        },\n        \"rate\": {\n          \"type\": \"string\",\n          \"description\": \"\
  Tax rate\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-tax-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Tax
---
