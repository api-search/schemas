---
description: Contact schema
layout: schema
name: Contact
properties_list:
- description: Contact phone number
  name: phoneNumber
  type: string
- description: Contact email
  name: email
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-contact-schema.json
slug: transfer-booking-contact
source_filename: transfer-booking-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"([+]?)[0-9]{1,20}\",\n      \"description\": \"Contact phone number\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Contact email\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-contact-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Contact
---
