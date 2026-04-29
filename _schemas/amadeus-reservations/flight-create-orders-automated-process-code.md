---
description: queuing action to be taken
layout: schema
name: AutomatedProcessCode
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-automated-process-code-schema.json
slug: flight-create-orders-automated-process-code
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-automated-process-code-schema.json\",\n  \"title\": \"AutomatedProcessCode\",\n  \"description\": \"queuing action to be taken\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"IMMEDIATE\",\n    \"DELAYED\",\n    \"ERROR\"\n  ],\n  \"example\": \"IMMEDIATE\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-automated-process-code-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AutomatedProcessCode
---
