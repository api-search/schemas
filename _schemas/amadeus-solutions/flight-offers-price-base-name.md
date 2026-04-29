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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-base-name-schema.json
slug: flight-offers-price-base-name
source_filename: flight-offers-price-base-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-base-name-schema.json\",\n  \"title\": \"BaseName\",\n  \"description\": \"description of the name of a physical person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"description\": \"First name.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"Last name.\",\n      \"type\": \"string\"\n    },\n    \"middleName\": {\n      \"description\": \"Middle name(s), for example \\\"Lee\\\" in \\\"John Lee Smith\\\".\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-base-name-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: BaseName
---
