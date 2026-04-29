---
description: Geolocation schema from Adyen API
layout: schema
name: Geolocation
properties_list:
- description: ''
  name: GeographicCoordinates
  type: object
- description: ''
  name: UTMCoordinates
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-geolocation-schema.json
slug: terminal-geolocation
source_filename: terminal-geolocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-geolocation-schema.json\",\n  \"title\": \"Geolocation\",\n  \"description\": \"Geolocation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GeographicCoordinates\": {\n      \"$ref\": \"#/components/schemas/GeographicCoordinates\"\n    },\n    \"UTMCoordinates\": {\n      \"$ref\": \"#/components/schemas/UTMCoordinates\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-geolocation-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Geolocation
---
