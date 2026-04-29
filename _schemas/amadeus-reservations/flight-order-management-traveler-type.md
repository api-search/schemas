---
description: 'traveler type age restrictions : CHILD < 12y, HELD_INFANT < 2y, SEATED_INFANT < 2y, SENIOR >=60y'
layout: schema
name: TravelerType
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-traveler-type-schema.json
slug: flight-order-management-traveler-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-traveler-type-schema.json\",\n  \"title\": \"TravelerType\",\n  \"description\": \"traveler type\\nage restrictions : CHILD < 12y, HELD_INFANT < 2y, SEATED_INFANT < 2y, SENIOR >=60y\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ADULT\",\n    \"CHILD\",\n    \"SENIOR\",\n    \"YOUNG\",\n    \"HELD_INFANT\",\n    \"SEATED_INFANT\",\n    \"STUDENT\"\n  ],\n  \"example\": \"ADULT\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-traveler-type-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TravelerType
---
