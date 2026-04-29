---
description: information returned in cancelation response
layout: schema
name: TransferCancellation
properties_list:
- description: transfer identifier - confirmation number from service provider that identifies the ride
  name: confirmNbr
  type: string
- description: status of reservation
  name: reservationStatus
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-management-transfer-cancellation-schema.json
slug: transfer-management-transfer-cancellation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-management-transfer-cancellation-schema.json\",\n  \"title\": \"TransferCancellation\",\n  \"description\": \"information returned in cancelation response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmNbr\": {\n      \"type\": \"string\",\n      \"description\": \"transfer identifier - confirmation number from service provider that identifies the ride\"\n    },\n    \"reservationStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CANCELLED\",\n        \"CONFIRMED\"\n      ],\n      \"description\": \"status of reservation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-management-transfer-cancellation-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TransferCancellation
---
