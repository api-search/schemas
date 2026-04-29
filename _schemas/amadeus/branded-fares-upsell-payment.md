---
description: ''
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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/branded-fares-upsell-payment-schema.json
slug: branded-fares-upsell-payment
source_filename: branded-fares-upsell-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Payment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"$ref\": \"#/definitions/PaymentBrand\"\n    },\n    \"binNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The first 6 digits of the credit card\"\n    },\n    \"flightOfferIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the flightOffers to pay\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/branded-fares-upsell-payment-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: Payment
---
