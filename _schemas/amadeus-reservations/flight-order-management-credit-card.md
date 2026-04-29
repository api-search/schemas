---
description: credit card
layout: schema
name: CreditCard
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-credit-card-schema.json
slug: flight-order-management-credit-card
source_filename: flight-order-management-credit-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-credit-card-schema.json\",\n  \"title\": \"CreditCard\",\n  \"description\": \"credit card\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/CreditCardCommon\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"securityCode\": {\n          \"description\": \"card security code\",\n          \"type\": \"string\",\n          \"example\": \"123\"\n        },\n        \"flightOfferIds\": {\n          \"description\": \"Id of the concern flightOffers\",\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"maxItems\": 6,\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": \"1\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-credit-card-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: CreditCard
---
