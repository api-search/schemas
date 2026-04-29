---
description: An individual address component of a geocoding result
layout: schema
name: AddressComponent
properties_list:
- description: The full text description of the address component
  name: long_name
  type: string
- description: An abbreviated textual name for the address component
  name: short_name
  type: string
- description: Array indicating the type of the address component
  name: types
  type: array
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-geocoding-address-component-schema.json
slug: google-maps-geocoding-address-component
source_filename: google-maps-geocoding-address-component-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddressComponent\",\n  \"type\": \"object\",\n  \"description\": \"An individual address component of a geocoding result\",\n  \"properties\": {\n    \"long_name\": {\n      \"type\": \"string\",\n      \"description\": \"The full text description of the address component\"\n    },\n    \"short_name\": {\n      \"type\": \"string\",\n      \"description\": \"An abbreviated textual name for the address component\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Array indicating the type of the address component\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-geocoding-address-component-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: AddressComponent
---
