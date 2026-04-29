---
description: ''
layout: schema
name: Issue
properties_list:
- description: the HTTP status code applicable to this error
  name: status
  type: integer
- description: an application-specific error code
  name: code
  type: integer
- description: a short summary of the error
  name: title
  type: string
- description: explanation of the error
  name: detail
  type: string
- description: an object containing references to the source of the error
  name: source
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-most-traveled-destinations-issue-schema.json
slug: flight-most-traveled-destinations-issue
source_filename: flight-most-traveled-destinations-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Issue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"the HTTP status code applicable to this error\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"an application-specific error code\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"a short summary of the error\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"explanation of the error\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"an object containing references to the source of the error\",\n      \"properties\": {\n        \"pointer\": {\n          \"type\": \"string\",\n          \"description\": \"a JSON Pointer [RFC6901] to the associated entity in the request document\"\n        },\n        \"parameter\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"a string indicating which URI query parameter caused the issue\"\n        },\n        \"example\": {\n          \"type\": \"string\",\n          \"description\": \"a string indicating an example of the right value\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-most-traveled-destinations-issue-schema.json
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
title: Issue
---
