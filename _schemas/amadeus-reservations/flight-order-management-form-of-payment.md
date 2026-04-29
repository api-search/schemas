---
description: form of payment used
layout: schema
name: FormOfPayment
properties_list:
- description: payment with the solution B2B Wallet
  name: b2bWallet
  type: object
- description: payment with a credit card
  name: creditCard
  type: object
- description: payment with an other method
  name: other
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-form-of-payment-schema.json
slug: flight-order-management-form-of-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-form-of-payment-schema.json\",\n  \"title\": \"FormOfPayment\",\n  \"description\": \"form of payment used\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"b2bWallet\": {\n      \"description\": \"payment with the solution B2B Wallet\",\n      \"$ref\": \"#/definitions/B2bWallet\"\n    },\n    \"creditCard\": {\n      \"description\": \"payment with a credit card\",\n      \"$ref\": \"#/definitions/CreditCard\"\n    },\n    \"other\": {\n      \"description\": \"payment with an other method\",\n      \"$ref\": \"#/definitions/OtherMethod\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-form-of-payment-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: FormOfPayment
---
