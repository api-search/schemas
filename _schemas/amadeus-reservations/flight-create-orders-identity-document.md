---
description: documents of the traveler
layout: schema
name: IdentityDocument
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-identity-document-schema.json
slug: flight-create-orders-identity-document
source_filename: flight-create-orders-identity-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-identity-document-schema.json\",\n  \"title\": \"IdentityDocument\",\n  \"description\": \"documents of the traveler\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Document\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"documentType\": {\n          \"$ref\": \"#/definitions/DocumentType\"\n        },\n        \"validityCountry\": {\n          \"type\": \"string\",\n          \"description\": \"[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) of the country where the document is valid\",\n          \"example\": \"IN\",\n          \"pattern\": \"[a-zA-Z]{2}\"\n        },\n        \"birthCountry\": {\n          \"type\": \"string\",\n          \"description\": \"[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)\
  \ of the country of birth\",\n          \"example\": \"FR\",\n          \"pattern\": \"[a-zA-Z]{2}\"\n        },\n        \"holder\": {\n          \"type\": \"boolean\",\n          \"description\": \"boolean to specify if the traveler is the holder of the document\",\n          \"example\": true\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-identity-document-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: IdentityDocument
---
