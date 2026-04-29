---
description: Markup applied to provide a service or a product to the client. The markup can be introduced by any stakeholder. Typical use case is to convey markup information set by the travel agent or in case of merchant mode.
layout: schema
name: Markup
properties_list:
- description: Defines the monetary value with decimal position as a String.
  name: amount
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-markup-schema.json
slug: hotel-search-markup
source_filename: hotel-search-markup-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Markup\",\n  \"description\": \"Markup applied to provide a service or a product to the client. The markup can be introduced by any stakeholder. Typical use case is to convey markup information set by the travel agent or in case of merchant mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Defines the monetary value with decimal position as a String.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-markup-schema.json
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
title: Markup
---
