---
description: ''
layout: schema
name: ErrorSource
properties_list:
- description: The key of the URI path or query parameter that caused the error
  name: parameter
  type: string
- description: A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error
  name: pointer
  type: string
- description: A sample input to guide the user when resolving this issue
  name: example
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-ratings-errorsource-schema.json
slug: hotel-ratings-errorsource
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ErrorSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameter\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the URI path or query parameter that caused the error\"\n    },\n    \"pointer\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error\"\n    },\n    \"example\": {\n      \"type\": \"string\",\n      \"description\": \"A sample input to guide the user when resolving this issue\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-ratings-errorsource-schema.json
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
title: ErrorSource
---
