---
description: loyalty program information
layout: schema
name: LoyaltyProgram
properties_list:
- description: loyalty program airline code
  name: programOwner
  type: string
- description: loyalty program number
  name: id
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-loyalty-program-schema.json
slug: flight-create-orders-loyalty-program
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-loyalty-program-schema.json\",\n  \"title\": \"LoyaltyProgram\",\n  \"description\": \"loyalty program information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"programOwner\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty program airline code\",\n      \"example\": \"AF\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty program number\",\n      \"example\": \"12357466574\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-loyalty-program-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: LoyaltyProgram
---
