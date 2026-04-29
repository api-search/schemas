---
description: Baggage schema
layout: schema
name: Baggage
properties_list:
- description: baggage capacity
  name: count
  type: integer
- description: baggage size code | name ------ | ---------------------------- S | Small M | Medium L | Large
  name: size
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-baggage-schema.json
slug: transfer-booking-baggage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-baggage-schema.json\",\n  \"title\": \"Baggage\",\n  \"description\": \"Baggage schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"baggage capacity\",\n      \"example\": 3\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"baggage size\\n\\ncode   | name                                 \\n------ | ---------------------------- \\nS \\t   | Small\\nM \\t   | Medium\\nL \\t   | Large\\n\",\n      \"enum\": [\n        \"S\",\n        \"M\",\n        \"L\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-baggage-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Baggage
---
