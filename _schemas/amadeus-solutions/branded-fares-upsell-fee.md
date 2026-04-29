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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-fee-schema.json
slug: branded-fares-upsell-fee
source_filename: branded-fares-upsell-fee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-fee-schema.json\",\n  \"title\": \"Fee\",\n  \"description\": \"a fee\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"example\": \"332.70\"\n    },\n    \"type\": {\n      \"$ref\": \"#/definitions/FeeType\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-fee-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Fee
---
