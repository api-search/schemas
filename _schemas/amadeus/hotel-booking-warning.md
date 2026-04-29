---
description: Warning
layout: schema
name: Warning
properties_list:
- description: '[Integer] A machine-readable warning code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of warning'
  name: code
  type: integer
- description: '[String] A warning title from the Canned Messages table with a 1:1 correspondence to the warning code. This may be localized'
  name: title
  type: string
- description: '[String] An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field value'
  name: detail
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-warning-schema.json
slug: hotel-booking-warning
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Warning\",\n  \"description\": \"Warning\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"[Integer] A machine-readable warning code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of warning\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"[String] A warning title from the Canned Messages table with a 1:1 correspondence to the warning code. This may be localized\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"[String] An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field value can be localized.\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-warning-schema.json
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
title: Warning
---
