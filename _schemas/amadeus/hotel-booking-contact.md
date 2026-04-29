---
description: Contact Details
layout: schema
name: Contact
properties_list:
- description: Phone Number in standard E.123(https://en.wikipedia.org/wiki/E.123)
  name: phone
  type: string
- description: Email Address
  name: email
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-contact-schema.json
slug: hotel-booking-contact
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact Details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone Number in standard E.123(https://en.wikipedia.org/wiki/E.123)\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email Address\"\n    }\n  },\n  \"required\": [\n    \"phone\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-contact-schema.json
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
