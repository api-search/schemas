---
description: description of the name of a physical person
layout: schema
name: BaseName
properties_list:
- description: First name.
  name: firstName
  type: string
- description: Last name.
  name: lastName
  type: string
- description: Middle name(s), for example "Lee" in "John Lee Smith".
  name: middleName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-basename-schema.json
slug: flight-offers-price-basename
source_filename: flight-offers-price-basename-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"BaseName\",\n  \"description\": \"description of the name of a physical person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name(s), for example \\\"Lee\\\" in \\\"John Lee Smith\\\".\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-basename-schema.json
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
title: BaseName
---
