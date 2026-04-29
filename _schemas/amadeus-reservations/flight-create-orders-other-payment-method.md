---
description: other payment method
layout: schema
name: OtherPaymentMethod
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-other-payment-method-schema.json
slug: flight-create-orders-other-payment-method
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-other-payment-method-schema.json\",\n  \"title\": \"OtherPaymentMethod\",\n  \"description\": \"other payment method\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACCOUNT\",\n    \"CHECK\",\n    \"CASH\",\n    \"NONREFUNDABLE\"\n  ],\n  \"example\": \"CASH\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-other-payment-method-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: OtherPaymentMethod
---
