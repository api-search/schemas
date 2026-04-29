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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-loyaltyprogram-schema.json
slug: seatmap-display-loyaltyprogram
source_filename: seatmap-display-loyaltyprogram-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LoyaltyProgram\",\n  \"description\": \"loyalty program information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"programOwner\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty program airline code\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"loyalty program number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-loyaltyprogram-schema.json
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
title: LoyaltyProgram
---
