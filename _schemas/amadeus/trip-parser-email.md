---
description: Email information.
layout: schema
name: email
properties_list:
- description: Category of the contact element
  name: category
  type: string
- description: Email address (e.g. john@smith.com)
  name: address
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-email-schema.json
slug: trip-parser-email
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"email\",\n  \"description\": \"Email information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the contact element\",\n      \"enum\": [\n        \"BUSINESS\",\n        \"PERSONAL\",\n        \"OTHER\"\n      ]\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Email address (e.g. john@smith.com)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-email-schema.json
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
title: email
---
