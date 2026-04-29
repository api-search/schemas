---
description: a tax
layout: schema
name: Tax
properties_list:
- description: ''
  name: amount
  type: string
- description: ''
  name: code
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-tax-schema.json
slug: flight-create-orders-tax
source_filename: flight-create-orders-tax-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-tax-schema.json\",\n  \"title\": \"Tax\",\n  \"description\": \"a tax\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"example\": \"332.70\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"example\": \"MX\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-tax-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Tax
---
