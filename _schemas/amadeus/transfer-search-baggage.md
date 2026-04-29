---
description: ''
layout: schema
name: Baggage
properties_list:
- description: baggage capacity
  name: count
  type: integer
- description: baggage size code | name | - S | Small M | Medium L | Large
  name: size
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-baggage-schema.json
slug: transfer-search-baggage
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Baggage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"baggage capacity\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"baggage size\\n\\ncode   | name                                 \\n | - \\nS \\t   | Small\\nM \\t   | Medium\\nL \\t   | Large\\n\",\n      \"enum\": [\n        \"S\",\n        \"M\",\n        \"L\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-baggage-schema.json
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
title: Baggage
---
