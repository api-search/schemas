---
description: ''
layout: schema
name: LoyaltyNumber
properties_list:
- description: loyalty program name
  name: program
  type: string
- description: loyalty number value
  name: value
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-loyaltynumber-schema.json
slug: transfer-booking-loyaltynumber
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LoyaltyNumber\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"program\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty program name\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty number value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-loyaltynumber-schema.json
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
title: LoyaltyNumber
---
