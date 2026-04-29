---
description: Guest Details
layout: schema
name: Stakeholder
properties_list:
- description: item identifier
  name: id
  type: integer
- description: ''
  name: name
  type: object
- description: ''
  name: contact
  type: object
- description: 'Hotel Chain Rewards Member Number. To receive your Rewards Points, access online check in, fast check out. An error is returned by the Chain if the number is invalid. Example Rewards Programs: * Marri'
  name: hotelRewardsMember
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-stakeholder-schema.json
slug: hotel-booking-stakeholder
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Stakeholder\",\n  \"description\": \"Guest Details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"item identifier\"\n    },\n    \"name\": {\n      \"$ref\": \"#/definitions/Name\"\n    },\n    \"contact\": {\n      \"$ref\": \"#/definitions/Contact\"\n    },\n    \"hotelRewardsMember\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel Chain Rewards Member Number. To receive your Rewards Points, access online check in, fast check out. An error is returned by the Chain if the number is invalid.\\nExample Rewards Programs:\\n* Marriott Bonvoy\\n* Hilton Honors\\n* Hyatt Rewards\\n* IHG Rewards\\n* Wyndham Rewards\\n* Accor Live Limitless ALL\\n* Best Western Rewards\\n* Choice Privileges\\n* Radisson Rewards\\n\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"contact\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-stakeholder-schema.json
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
title: Stakeholder
---
