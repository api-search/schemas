---
description: Agency email information.
layout: schema
name: Agency
properties_list:
- description: List of contact information
  name: contacts
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-agency-schema.json
slug: transfer-booking-agency
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Agency\",\n  \"description\": \"Agency email information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contacts\": {\n      \"type\": \"array\",\n      \"description\": \"List of contact information\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"email\": {\n            \"type\": \"object\",\n            \"description\": \"Email information.\",\n            \"properties\": {\n              \"address\": {\n                \"type\": \"string\",\n                \"format\": \"email\",\n                \"description\": \"Email address (e.g. john@smith.com)\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-agency-schema.json
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
title: Agency
---
