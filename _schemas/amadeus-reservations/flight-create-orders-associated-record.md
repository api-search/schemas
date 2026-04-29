---
description: record associated to the order
layout: schema
name: AssociatedRecord
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-associated-record-schema.json
slug: flight-create-orders-associated-record
source_filename: flight-create-orders-associated-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-associated-record-schema.json\",\n  \"title\": \"AssociatedRecord\",\n  \"description\": \"record associated to the order\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/AssociatedRecordCommon\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"flightOfferId\": {\n          \"type\": \"string\",\n          \"description\": \"id of the impacted flight offer\",\n          \"example\": \"1\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-associated-record-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AssociatedRecord
---
