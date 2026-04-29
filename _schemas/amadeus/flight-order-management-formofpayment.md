---
description: form of payment used
layout: schema
name: FormOfPayment
properties_list:
- description: ''
  name: b2bWallet
  type: object
- description: ''
  name: creditCard
  type: object
- description: ''
  name: other
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-formofpayment-schema.json
slug: flight-order-management-formofpayment
source_filename: flight-order-management-formofpayment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FormOfPayment\",\n  \"description\": \"form of payment used\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"b2bWallet\": {\n      \"$ref\": \"#/definitions/B2bWallet\"\n    },\n    \"creditCard\": {\n      \"$ref\": \"#/definitions/CreditCard\"\n    },\n    \"other\": {\n      \"$ref\": \"#/definitions/OtherMethod\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-formofpayment-schema.json
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
title: FormOfPayment
---
