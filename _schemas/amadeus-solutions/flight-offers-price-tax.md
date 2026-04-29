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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-tax-schema.json
slug: flight-offers-price-tax
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-tax-schema.json\",\n  \"title\": \"Tax\",\n  \"description\": \"a tax\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"example\": \"332.70\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"example\": \"MX\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-tax-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Tax
---
