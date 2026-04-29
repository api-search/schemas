---
description: Specific type to convey a list of string for specific information type ( via qualifier) in specific character set, or language
layout: schema
name: description
properties_list:
- description: Free Text
  name: text
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-description-schema.json
slug: trip-parser-description
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"description\",\n  \"description\": \"\\t\\nSpecific type to convey a list of string for specific information type ( via qualifier) in specific character set, or language\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Free Text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-description-schema.json
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
title: description
---
