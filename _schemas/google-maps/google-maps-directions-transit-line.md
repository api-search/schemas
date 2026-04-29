---
description: Information about a transit line
layout: schema
name: TransitLine
properties_list:
- description: The full name of this transit line
  name: name
  type: string
- description: The short name of this transit line
  name: short_name
  type: string
- description: The color commonly used in signage for this line
  name: color
  type: string
- description: The color of the text commonly used for this line
  name: text_color
  type: string
- description: ''
  name: vehicle
  type: object
- description: ''
  name: agencies
  type: array
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-transit-line-schema.json
slug: google-maps-directions-transit-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransitLine\",\n  \"type\": \"object\",\n  \"description\": \"Information about a transit line\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of this transit line\"\n    },\n    \"short_name\": {\n      \"type\": \"string\",\n      \"description\": \"The short name of this transit line\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"The color commonly used in signage for this line\"\n    },\n    \"text_color\": {\n      \"type\": \"string\",\n      \"description\": \"The color of the text commonly used for this line\"\n    },\n    \"vehicle\": {\n      \"type\": \"object\"\n    },\n    \"agencies\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-transit-line-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: TransitLine
---
