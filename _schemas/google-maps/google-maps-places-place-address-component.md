---
description: An address component of a place
layout: schema
name: PlaceAddressComponent
properties_list:
- description: The full text of the address component
  name: longText
  type: string
- description: An abbreviated text for the address component
  name: shortText
  type: string
- description: The types of this address component
  name: types
  type: array
- description: The language code for this component
  name: languageCode
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-place-address-component-schema.json
slug: google-maps-places-place-address-component
source_filename: google-maps-places-place-address-component-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlaceAddressComponent\",\n  \"type\": \"object\",\n  \"description\": \"An address component of a place\",\n  \"properties\": {\n    \"longText\": {\n      \"type\": \"string\",\n      \"description\": \"The full text of the address component\"\n    },\n    \"shortText\": {\n      \"type\": \"string\",\n      \"description\": \"An abbreviated text for the address component\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"The types of this address component\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language code for this component\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-place-address-component-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: PlaceAddressComponent
---
