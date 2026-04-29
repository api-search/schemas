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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-credit-card-common-schema.json
slug: flight-create-orders-credit-card-common
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-credit-card-common-schema.json\",\n  \"title\": \"CreditCardCommon\",\n  \"description\": \"credit card common attribute\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"$ref\": \"#/definitions/CreditCardBrand\"\n    },\n    \"holder\": {\n      \"description\": \"card holder as on the card\",\n      \"type\": \"string\",\n      \"example\": \"MR DUPON DAMIEN\"\n    },\n    \"number\": {\n      \"description\": \"card number\",\n      \"type\": \"string\",\n      \"example\": \"4012999999999999\",\n      \"pattern\": \"[a-zA-Z0-9]{1,35}\"\n    },\n    \"expiryDate\": {\n      \"description\": \"credit card expiration date following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) (YYYY-MM format, e.g. 2012-08)\",\n      \"type\": \"string\",\n    \
  \  \"example\": \"2021-08\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-credit-card-common-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: CreditCardCommon
---
