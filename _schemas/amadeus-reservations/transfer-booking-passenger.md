---
description: passenger data
layout: schema
name: Passenger
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-passenger-schema.json
slug: transfer-booking-passenger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-passenger-schema.json\",\n  \"title\": \"Passenger\",\n  \"description\": \"passenger data\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Name\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contacts\": {\n          \"$ref\": \"#/definitions/Contact\"\n        },\n        \"billingAddress\": {\n          \"$ref\": \"#/definitions/AddressCommon\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-passenger-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Passenger
---
