---
description: Payment schema
layout: schema
name: Payment
properties_list:
- description: ''
  name: brand
  type: object
- description: The first 6 digits of the credit card
  name: binNumber
  type: integer
- description: Id of the flightOffers to pay
  name: flightOfferIds
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-payment-schema.json
slug: branded-fares-upsell-payment
source_filename: branded-fares-upsell-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-payment-schema.json\",\n  \"title\": \"Payment\",\n  \"description\": \"Payment schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"$ref\": \"#/definitions/PaymentBrand\"\n    },\n    \"binNumber\": {\n      \"description\": \"The first 6 digits of the credit card\",\n      \"type\": \"integer\",\n      \"example\": 123456,\n      \"pattern\": \"[0-9]{6}\"\n    },\n    \"flightOfferIds\": {\n      \"description\": \"Id of the flightOffers to pay\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-payment-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Payment
---
