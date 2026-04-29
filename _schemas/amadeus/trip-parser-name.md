---
description: Description of the name of a physical person
layout: schema
name: name
properties_list:
- description: First name.
  name: firstName
  type: string
- description: Last name.
  name: lastName
  type: string
- description: Contains all the suffixes and prefixes that can be appended to a name - Mr, Miss, Pr. - E.g. " Mr".
  name: title
  type: string
- description: Middle name(s), for example "Lee" in "John Lee Smith".
  name: middleName
  type: string
- description: Name prefix (e.g. Doctor)
  name: prefix
  type: string
- description: Name suffix (e.g. Junior, III, etc).
  name: suffix
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-name-schema.json
slug: trip-parser-name
source_filename: trip-parser-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"name\",\n  \"description\": \"Description of the name of a physical person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Contains all the suffixes and prefixes that can be appended to a name - Mr, Miss, Pr. - E.g. \\\" Mr\\\".\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name(s), for example \\\"Lee\\\" in \\\"John Lee Smith\\\".\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Name prefix (e.g. Doctor)\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"Name suffix (e.g. Junior, III, etc).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-name-schema.json
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
title: name
---
