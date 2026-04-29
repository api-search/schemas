---
description: Associated Record (Flight Booking Record)
layout: schema
name: AssociatedRecord
properties_list:
- description: Amadeus GDS Record
  name: reference
  type: string
- description: '* GDS: Associated Amadeus GDS Flight Booking PNR Record'
  name: originSystemCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-associatedrecord-schema.json
slug: hotel-booking-associatedrecord
source_filename: hotel-booking-associatedrecord-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AssociatedRecord\",\n  \"description\": \"Associated Record (Flight Booking Record)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Amadeus GDS Record\"\n    },\n    \"originSystemCode\": {\n      \"type\": \"string\",\n      \"description\": \"* GDS: Associated Amadeus GDS Flight Booking PNR Record\",\n      \"enum\": [\n        \"GDS\"\n      ]\n    }\n  },\n  \"required\": [\n    \"reference\",\n    \"originSystemCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-associatedrecord-schema.json
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
title: AssociatedRecord
---
