---
description: Text with structured formatting information
layout: schema
name: FormattableText
properties_list:
- description: The full text string
  name: text
  type: string
- description: List of string ranges identifying where the input request matched in the text
  name: matches
  type: array
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-formattable-text-schema.json
slug: google-maps-places-formattable-text
source_filename: google-maps-places-formattable-text-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FormattableText\",\n  \"type\": \"object\",\n  \"description\": \"Text with structured formatting information\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The full text string\"\n    },\n    \"matches\": {\n      \"type\": \"array\",\n      \"description\": \"List of string ranges identifying where the input request matched in the text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-formattable-text-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: FormattableText
---
