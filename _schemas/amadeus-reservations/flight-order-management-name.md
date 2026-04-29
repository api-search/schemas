---
description: name
layout: schema
name: Name
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-name-schema.json
slug: flight-order-management-name
source_filename: flight-order-management-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-name-schema.json\",\n  \"title\": \"Name\",\n  \"description\": \"name\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/BaseName\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"secondLastName\": {\n          \"description\": \"second last name\",\n          \"type\": \"string\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-name-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Name
---
