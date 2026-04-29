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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-qualifiedfreetext-schema.json
slug: seatmap-display-qualifiedfreetext
source_filename: seatmap-display-qualifiedfreetext-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"QualifiedFreeText\",\n  \"description\": \"Specific type to convey a list of string for specific information type ( via qualifier) in specific character set, or language\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Free Text\"\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"see RFC 5646\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-qualifiedfreetext-schema.json
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
title: QualifiedFreeText
---
