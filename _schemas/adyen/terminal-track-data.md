---
description: ISO 7813 - ISO 4909. Generic data structure for a card track, used when the magstripe card reader is located on the Sale Terminal, or for magstripe Card Reader device request. The data structure is also used to store the line at the bottom of a bank check. Magnetic track or magnetic ink characters line.
layout: schema
name: TrackData
properties_list:
- description: ''
  name: TrackNumb
  type: integer
- description: ''
  name: TrackFormat
  type: object
- description: ''
  name: TrackValue
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-track-data-schema.json
slug: terminal-track-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-track-data-schema.json\",\n  \"title\": \"TrackData\",\n  \"description\": \"ISO 7813 - ISO 4909.  Generic data structure for a card track, used when the magstripe card reader is located on the Sale Terminal, or for magstripe Card Reader device request. The data structure is also used to store the line at the bottom of a bank check. Magnetic track or magnetic ink characters line.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TrackNumb\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 3,\n      \"default\": 2\n    },\n    \"TrackFormat\": {\n      \"$ref\": \"#/components/schemas/TrackFormat\"\n    },\n    \"TrackValue\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,104}$\"\n    }\n  },\n  \"required\": [\n    \"TrackValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-track-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TrackData
---
