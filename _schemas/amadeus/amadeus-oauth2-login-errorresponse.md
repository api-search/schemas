---
description: Error responses are sent when an error (e.g. unauthorized, bad request, ...) occurred.
layout: schema
name: ErrorResponse
properties_list:
- description: Name is the error name.
  name: error
  type: string
- description: A small description about the error
  name: error_description
  type: string
- description: Debug contains debug information.
  name: code
  type: integer
- description: Debug contains debug information. This is usually not available and has to be enabled.
  name: title
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/amadeus-oauth2-login-errorresponse-schema.json
slug: amadeus-oauth2-login-errorresponse
source_filename: amadeus-oauth2-login-errorresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Error responses are sent when an error (e.g. unauthorized, bad request, ...) occurred.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Name is the error name.\"\n    },\n    \"error_description\": {\n      \"type\": \"string\",\n      \"description\": \"A small description about the error\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Debug contains debug information.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Debug contains debug information. This is usually not available and has to be enabled.\"\n    }\n  },\n  \"required\": [\n    \"error\",\n    \"error_description\",\n    \"code\",\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/amadeus-oauth2-login-errorresponse-schema.json
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
title: ErrorResponse
---
