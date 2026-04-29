---
description: Issue schema
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-issue-schema.json
slug: branded-fares-upsell-issue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-issue-schema.json\",\n  \"title\": \"Issue\",\n  \"description\": \"Issue schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"description\": \"the HTTP status code applicable to this error\",\n      \"type\": \"integer\"\n    },\n    \"code\": {\n      \"description\": \"an application-specific error code\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"title\": {\n      \"description\": \"a short summary of the error\",\n      \"type\": \"string\"\n    },\n    \"detail\": {\n      \"description\": \"explanation of the error\",\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"title\": \"Issue_Source\",\n      \"description\": \"an object containing references to the source of the\
  \ error\",\n      \"maxProperties\": 1,\n      \"properties\": {\n        \"pointer\": {\n          \"description\": \"a JSON Pointer [RFC6901] to the associated entity in the request document\",\n          \"type\": \"string\"\n        },\n        \"parameter\": {\n          \"description\": \"a string indicating which URI query parameter caused the issue\",\n          \"type\": \"string\"\n        },\n        \"example\": {\n          \"description\": \"a string indicating an example of the right value\",\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-issue-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Issue
---
