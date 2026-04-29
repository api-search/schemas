---
description: transfer reservation
layout: schema
name: TransferReservation
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-transfer-reservation-schema.json
slug: transfer-booking-transfer-reservation
source_filename: transfer-booking-transfer-reservation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-transfer-reservation-schema.json\",\n  \"title\": \"TransferReservation\",\n  \"description\": \"transfer reservation\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"confirmNbr\": {\n          \"type\": \"string\",\n          \"description\": \"transfer identifier - confirmation number, received from transfer supplier\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"status of transfer reservation\",\n          \"enum\": [\n            \"CONFIRMED\",\n            \"CANCELLED\"\n          ]\n        },\n        \"note\": {\n          \"type\": \"string\",\n          \"description\": \"Note to transfer provider\"\n        },\n        \"methodOfPayment\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Method of payment required when PaymentType equal BT (applicable only for reservation action).\",\n          \"enum\": [\n            \"CREDIT_CARD\",\n            \"INVOICE\",\n            \"TRAVEL_ACCOUNT\",\n            \"PAYMENT_SERVICE_PROVIDER\"\n          ]\n        },\n        \"paymentServiceProvider\": {\n          \"type\": \"string\",\n          \"description\": \"payment service provider details will be passed to provider in case \\\"PAYMENT_SERVICE_PROVIDER\\\" method of payment.\",\n          \"enum\": [\n            \"STRIPE_CONNECT\"\n          ]\n        },\n        \"offerId\": {\n          \"type\": \"string\",\n          \"description\": \"offer identifier\"\n        }\n      }\n    },\n    {\n      \"$ref\": \"#/definitions/Transfer\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-transfer-reservation-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TransferReservation
---
