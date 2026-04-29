---
description: UTMCoordinates schema from Adyen API
layout: schema
name: UTMCoordinates
properties_list:
- description: ''
  name: UTMZone
  type: string
- description: ''
  name: UTMEastward
  type: string
- description: ''
  name: UTMNorthward
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-utm-coordinates-schema.json
slug: terminal-utm-coordinates
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-utm-coordinates-schema.json\",\n  \"title\": \"UTMCoordinates\",\n  \"description\": \"UTMCoordinates schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UTMZone\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"UTMEastward\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"UTMNorthward\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"UTMZone\",\n    \"UTMEastward\",\n    \"UTMNorthward\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-utm-coordinates-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UTMCoordinates
---
