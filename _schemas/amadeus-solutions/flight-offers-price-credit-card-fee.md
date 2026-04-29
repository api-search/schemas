---
description: CreditCardFee schema
layout: schema
name: CreditCardFee
properties_list:
- description: ''
  name: brand
  type: object
- description: ''
  name: amount
  type: string
- description: ''
  name: currency
  type: string
- description: Id of the flightOffer concerned by the credit card fee
  name: flightOfferId
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-credit-card-fee-schema.json
slug: flight-offers-price-credit-card-fee
source_filename: flight-offers-price-credit-card-fee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-credit-card-fee-schema.json\",\n  \"title\": \"CreditCardFee\",\n  \"description\": \"CreditCardFee schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"$ref\": \"#/definitions/PaymentBrand\"\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"example\": \"1\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"example\": \"USD\"\n    },\n    \"flightOfferId\": {\n      \"description\": \"Id of the flightOffer concerned by the credit card fee\",\n      \"type\": \"string\",\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-credit-card-fee-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: CreditCardFee
---
