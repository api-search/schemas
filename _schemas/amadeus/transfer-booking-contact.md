---
description: ''
layout: schema
name: Contact
properties_list:
- description: Contact phone number
  name: phoneNumber
  type: string
- description: Contact email
  name: email
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-contact-schema.json
slug: transfer-booking-contact
source_filename: transfer-booking-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Contact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Contact phone number\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Contact email\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-contact-schema.json
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
title: Contact
---
