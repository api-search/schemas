---
description: Details of chargeable seat
layout: schema
name: ChargeableSeat
properties_list:
- description: Id of the chargeable seat
  name: id
  type: string
- description: seat number
  name: number
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-chargeable-seat-schema.json
slug: flight-create-orders-chargeable-seat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-chargeable-seat-schema.json\",\n  \"title\": \"ChargeableSeat\",\n  \"description\": \"Details of chargeable seat\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Id of the chargeable seat\",\n      \"type\": \"string\",\n      \"example\": \"1\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"seat number\",\n      \"example\": \"33D\",\n      \"pattern\": \"[1-9][0-9]{0,2}[A-Z]?\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-chargeable-seat-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: ChargeableSeat
---
