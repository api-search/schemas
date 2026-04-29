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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-management-transfercancellation-schema.json
slug: transfer-management-transfercancellation
source_filename: transfer-management-transfercancellation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TransferCancellation\",\n  \"description\": \"information returned in cancelation response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmNbr\": {\n      \"type\": \"string\",\n      \"description\": \"transfer identifier - confirmation number from service provider that identifies the ride\"\n    },\n    \"reservationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"status of reservation\",\n      \"enum\": [\n        \"CANCELLED\",\n        \"CONFIRMED\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-management-transfercancellation-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: TransferCancellation
---
