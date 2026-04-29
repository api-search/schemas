---
description: defines the payment in transfer reservation. For "CREDIT_CARD" - creditCard is mandatory, for "TRAVEL_ACCOUNT" - paymentReference is optional, for "PAYMENT_SERVICE_PROVIDER" - paymentServiceProvider and paymentReference are mandatory.
layout: schema
name: Payment
properties_list:
- description: Method of payment required when PaymentType equal BT (applicable only for reservation action).
  name: methodOfPayment
  type: string
- description: payment refence that will be passed to provider in case "TRAVEL_ACCOUNT" method of payment
  name: paymentReference
  type: string
- description: payment service provider details will be passed to provider in case "PAYMENT_SERVICE_PROVIDER" method of payment.
  name: paymentServiceProvider
  type: string
- description: ''
  name: creditCard
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-payment-schema.json
slug: transfer-booking-payment
source_filename: transfer-booking-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-payment-schema.json\",\n  \"title\": \"Payment\",\n  \"description\": \"defines the payment in transfer reservation. For \\\"CREDIT_CARD\\\" - creditCard is mandatory, for \\\"TRAVEL_ACCOUNT\\\" - paymentReference is optional, for \\\"PAYMENT_SERVICE_PROVIDER\\\" - paymentServiceProvider and paymentReference are mandatory.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"methodOfPayment\": {\n      \"type\": \"string\",\n      \"description\": \"Method of payment required when PaymentType equal BT (applicable only for reservation action).\",\n      \"enum\": [\n        \"CREDIT_CARD\",\n        \"TRAVEL_ACCOUNT\",\n        \"PAYMENT_SERVICE_PROVIDER\"\n      ]\n    },\n    \"paymentReference\": {\n      \"type\": \"string\",\n      \"description\": \"payment refence that\
  \ will be passed to provider in case \\\"TRAVEL_ACCOUNT\\\" method of payment\"\n    },\n    \"paymentServiceProvider\": {\n      \"type\": \"string\",\n      \"description\": \"payment service provider details will be passed to provider in case \\\"PAYMENT_SERVICE_PROVIDER\\\" method of payment.\",\n      \"enum\": [\n        \"STRIPE_CONNECT\"\n      ]\n    },\n    \"creditCard\": {\n      \"$ref\": \"#/definitions/CreditCard\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-payment-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Payment
---
