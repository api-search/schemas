---
description: other payment method
layout: schema
name: OtherMethod
properties_list:
- description: ''
  name: method
  type: object
- description: Id of the concern flightOffers
  name: flightOfferIds
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-other-method-schema.json
slug: flight-create-orders-other-method
source_filename: flight-create-orders-other-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-other-method-schema.json\",\n  \"title\": \"OtherMethod\",\n  \"description\": \"other payment method\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"$ref\": \"#/definitions/OtherPaymentMethod\"\n    },\n    \"flightOfferIds\": {\n      \"description\": \"Id of the concern flightOffers\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-other-method-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: OtherMethod
---
