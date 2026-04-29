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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-name-schema.json
slug: transfer-booking-name
source_filename: transfer-booking-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-name-schema.json\",\n  \"title\": \"Name\",\n  \"description\": \"description of the name of a physical person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"The type of the Name\",\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"description\": \"First name.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"Last name.\",\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"description\": \"Contains all the suffixes and prefixes that can be appended to a name - Mr, Miss, Pr. - E.g. \\\" Mr\\\".\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-name-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Name
---
