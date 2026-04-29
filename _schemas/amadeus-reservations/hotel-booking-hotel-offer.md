---
description: Hotel Offer
layout: schema
name: HotelOffer
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-hotel-offer-schema.json
slug: hotel-booking-hotel-offer
source_filename: hotel-booking-hotel-offer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-offer-schema.json\",\n  \"title\": \"HotelOffer\",\n  \"description\": \"Hotel Offer\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"description\": \"data type set to hotel-offer\",\n          \"type\": \"string\",\n          \"example\": \"hotel-offer\",\n          \"default\": \"hotel-offer\",\n          \"enum\": [\n            \"hotel-offer\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z0-9]*$\",\n          \"minLength\": 2,\n          \"maxLength\": 100,\n          \"example\": \"63A93695B58821ABB0EC2B33FE9FAB24D72BF34B1BD7D707293763D8D9378FC3\",\n          \"description\": \"Unique identifier of this offer. Might be valid for a temporary period\
  \ only.\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    {\n      \"$ref\": \"#/definitions/HotelProduct\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-offer-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: HotelOffer
---
