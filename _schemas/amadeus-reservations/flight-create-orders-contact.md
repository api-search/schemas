---
description: contact information
layout: schema
name: Contact
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-contact-schema.json
slug: flight-create-orders-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"contact information\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/ContactDictionary\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"phones\": {\n          \"description\": \"Phone numbers\",\n          \"type\": \"array\",\n          \"maxItems\": 3,\n          \"items\": {\n            \"$ref\": \"#/definitions/Phone\"\n          }\n        },\n        \"companyName\": {\n          \"description\": \"Name of the company\",\n          \"type\": \"string\",\n          \"example\": \"AMADEUS\"\n        },\n        \"emailAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Email address (e.g. john@smith.com)\",\n          \"example\": \"support@mail.com\"\
  \n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-contact-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Contact
---
