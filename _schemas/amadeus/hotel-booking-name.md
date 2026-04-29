---
description: Guest Name
layout: schema
name: Name
properties_list:
- description: title/gender of room guest
  name: title
  type: string
- description: first name (and middle name) of room guest
  name: firstName
  type: string
- description: last name of room guest
  name: lastName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-name-schema.json
slug: hotel-booking-name
source_filename: hotel-booking-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Name\",\n  \"description\": \"Guest Name\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"title/gender of room guest\",\n      \"enum\": [\n        \"MR\",\n        \"MRS\",\n        \"MS\"\n      ]\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"first name (and middle name) of room guest\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"last name of room guest\"\n    }\n  },\n  \"required\": [\n    \"firstName\",\n    \"lastName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-name-schema.json
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
title: Name
---
