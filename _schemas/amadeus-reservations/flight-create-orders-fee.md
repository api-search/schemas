---
description: a fee
layout: schema
name: Fee
properties_list:
- description: ''
  name: amount
  type: string
- description: ''
  name: type
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-fee-schema.json
slug: flight-create-orders-fee
source_filename: flight-create-orders-fee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-fee-schema.json\",\n  \"title\": \"Fee\",\n  \"description\": \"a fee\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"example\": \"332.70\"\n    },\n    \"type\": {\n      \"$ref\": \"#/definitions/FeeType\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-fee-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Fee
---
