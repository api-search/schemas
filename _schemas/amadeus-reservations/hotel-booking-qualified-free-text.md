---
description: Specific type to convey a list of string for specific information type ( via qualifier) in specific character set, or language
layout: schema
name: QualifiedFreeText
properties_list:
- description: Free Text
  name: text
  type: string
- description: see RFC 5646
  name: lang
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-qualified-free-text-schema.json
slug: hotel-booking-qualified-free-text
source_filename: hotel-booking-qualified-free-text-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-qualified-free-text-schema.json\",\n  \"title\": \"QualifiedFreeText\",\n  \"description\": \"Specific type to convey a list of string for specific information type ( via qualifier) in specific character set, or language\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Free Text\",\n      \"example\": \"Do you need and example ?\"\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"see RFC 5646\",\n      \"example\": \"fr-FR\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-qualified-free-text-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: QualifiedFreeText
---
