---
description: Contact and Adress details
layout: schema
name: ContactWithAddress
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-contact-with-address-schema.json
slug: transfer-booking-contact-with-address
source_filename: transfer-booking-contact-with-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-contact-with-address-schema.json\",\n  \"title\": \"ContactWithAddress\",\n  \"description\": \"Contact and Adress details\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Contact\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address\": {\n          \"$ref\": \"#/definitions/AddressCommon\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-contact-with-address-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: ContactWithAddress
---
