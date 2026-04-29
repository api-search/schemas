---
description: An encoded location reference, derived from latitude and longitude coordinates, that represents an area. Plus codes can be used as a replacement for street addresses in places where they do not exist.
layout: schema
name: PlusCode
properties_list:
- description: The global (full) plus code consisting of area code and local code (e.g., 849VCWC8+R9).
  name: global_code
  type: string
- description: The compound plus code consisting of the local code and a locality description (e.g., CWC8+R9 Mountain View, CA, USA).
  name: compound_code
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-geocoding-plus-code-schema.json
slug: google-maps-geocoding-plus-code
source_filename: google-maps-geocoding-plus-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlusCode\",\n  \"type\": \"object\",\n  \"description\": \"An encoded location reference, derived from latitude and longitude coordinates, that represents an area. Plus codes can be used as a replacement for street addresses in places where they do not exist.\",\n  \"properties\": {\n    \"global_code\": {\n      \"type\": \"string\",\n      \"description\": \"The global (full) plus code consisting of area code and local code (e.g., 849VCWC8+R9).\"\n    },\n    \"compound_code\": {\n      \"type\": \"string\",\n      \"description\": \"The compound plus code consisting of the local code and a locality description (e.g., CWC8+R9 Mountain View, CA, USA).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-geocoding-plus-code-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: PlusCode
---
