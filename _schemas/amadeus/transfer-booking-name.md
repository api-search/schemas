---
description: description of the name of a physical person
layout: schema
name: Name
properties_list:
- description: The type of the Name
  name: type
  type: string
- description: First name.
  name: firstName
  type: string
- description: Last name.
  name: lastName
  type: string
- description: Contains all the suffixes and prefixes that can be appended to a name - Mr, Miss, Pr. - E.g. " Mr".
  name: title
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-name-schema.json
slug: transfer-booking-name
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Name\",\n  \"description\": \"description of the name of a physical person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the Name\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Contains all the suffixes and prefixes that can be appended to a name - Mr, Miss, Pr. - E.g. \\\" Mr\\\".\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-name-schema.json
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
