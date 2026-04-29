---
description: credit card common attribute
layout: schema
name: CreditCardCommon
properties_list:
- description: ''
  name: brand
  type: object
- description: card holder as on the card
  name: holder
  type: string
- description: card number
  name: number
  type: string
- description: credit card expiration date following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) (YYYY-MM format, e.g. 2012-08)
  name: expiryDate
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-creditcardcommon-schema.json
slug: flight-order-management-creditcardcommon
source_filename: flight-order-management-creditcardcommon-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreditCardCommon\",\n  \"description\": \"credit card common attribute\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"$ref\": \"#/definitions/CreditCardBrand\"\n    },\n    \"holder\": {\n      \"type\": \"string\",\n      \"description\": \"card holder as on the card\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"card number\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"credit card expiration date following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) (YYYY-MM format, e.g. 2012-08)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-creditcardcommon-schema.json
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
title: CreditCardCommon
---
