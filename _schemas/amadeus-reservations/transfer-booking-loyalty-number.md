---
description: LoyaltyNumber schema
layout: schema
name: LoyaltyNumber
properties_list:
- description: loyalty program name
  name: program
  type: string
- description: loyalty number value
  name: value
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-loyalty-number-schema.json
slug: transfer-booking-loyalty-number
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-loyalty-number-schema.json\",\n  \"title\": \"LoyaltyNumber\",\n  \"description\": \"LoyaltyNumber schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"program\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty program name\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty number value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-loyalty-number-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: LoyaltyNumber
---
