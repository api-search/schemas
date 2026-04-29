---
description: Payment options accepted by a place
layout: schema
name: PaymentOptions
properties_list:
- description: ''
  name: acceptsCreditCards
  type: boolean
- description: ''
  name: acceptsDebitCards
  type: boolean
- description: ''
  name: acceptsCashOnly
  type: boolean
- description: ''
  name: acceptsNfc
  type: boolean
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-payment-options-schema.json
slug: google-maps-places-payment-options
source_filename: google-maps-places-payment-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentOptions\",\n  \"type\": \"object\",\n  \"description\": \"Payment options accepted by a place\",\n  \"properties\": {\n    \"acceptsCreditCards\": {\n      \"type\": \"boolean\"\n    },\n    \"acceptsDebitCards\": {\n      \"type\": \"boolean\"\n    },\n    \"acceptsCashOnly\": {\n      \"type\": \"boolean\"\n    },\n    \"acceptsNfc\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-payment-options-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: PaymentOptions
---
