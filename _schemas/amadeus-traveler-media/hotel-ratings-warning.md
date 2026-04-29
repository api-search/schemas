---
description: Warning schema
layout: schema
name: Warning
properties_list:
- description: A machine-readable error code from the Canned Messages table, that will enable the API Consumers code to handle this type of error
  name: code
  type: integer
- description: An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized
  name: title
  type: string
- description: An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field’s value can be
  name: detail
  type: string
- description: ''
  name: source
  type: object
- description: A link to a web page or file with further documentation to help the API consumer resolve this error
  name: documentation
  type: string
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/hotel-ratings-warning-schema.json
slug: hotel-ratings-warning
source_filename: hotel-ratings-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-warning-schema.json\",\n  \"title\": \"Warning\",\n  \"description\": \"Warning schema\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"A machine-readable error code from the Canned Messages table, that will enable the API Consumers code to handle this type of error\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field\\u2019s value\
  \ can be localized.\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/ErrorSource\"\n    },\n    \"documentation\": {\n      \"type\": \"string\",\n      \"format\": \"url\",\n      \"description\": \"A link to a web page or file with further documentation to help the API consumer resolve this error\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"title\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-warning-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Warning
---
