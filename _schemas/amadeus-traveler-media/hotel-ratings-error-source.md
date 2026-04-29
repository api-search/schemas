---
description: ErrorSource schema
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
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/hotel-ratings-error-source-schema.json
slug: hotel-ratings-error-source
source_filename: hotel-ratings-error-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-error-source-schema.json\",\n  \"title\": \"ErrorSource\",\n  \"description\": \"ErrorSource schema\",\n  \"properties\": {\n    \"parameter\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the URI path or query parameter that caused the error\"\n    },\n    \"pointer\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error\"\n    },\n    \"example\": {\n      \"type\": \"string\",\n      \"description\": \"A sample input to guide the user when resolving this issue\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/hotel-ratings-error-source-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: ErrorSource
---
