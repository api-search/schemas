---
description: quality of service offered in the cabin where the seat is located in this flight. Economy, premium economy, business or first class
layout: schema
name: TravelClass
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-travel-class-schema.json
slug: flight-create-orders-travel-class
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-travel-class-schema.json\",\n  \"title\": \"TravelClass\",\n  \"description\": \"quality of service offered in the cabin where the seat is located in this flight. Economy, premium economy, business or first class\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ECONOMY\",\n    \"PREMIUM_ECONOMY\",\n    \"BUSINESS\",\n    \"FIRST\"\n  ],\n  \"example\": \"PREMIUM_ECONOMY\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-travel-class-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TravelClass
---
