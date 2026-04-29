---
description: the nature/type of the document
layout: schema
name: DocumentType
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-document-type-schema.json
slug: flight-create-orders-document-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-document-type-schema.json\",\n  \"title\": \"DocumentType\",\n  \"description\": \"the nature/type of the document\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"VISA\",\n    \"PASSPORT\",\n    \"IDENTITY_CARD\",\n    \"KNOWN_TRAVELER\",\n    \"REDRESS\"\n  ],\n  \"example\": \"VISA\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-document-type-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: DocumentType
---
