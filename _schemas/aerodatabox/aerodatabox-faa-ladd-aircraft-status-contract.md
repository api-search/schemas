---
description: Status of the aircraft tail number or callsign in the FAA Limiting Aircraft Data Displayed (LADD) Program list. See https://www.faa.gov/pilots/ladd for more details.
layout: schema
name: FaaLaddAircraftStatusContract
properties_list:
- description: ''
  name: id
  type: string
- description: Current status of the aircraft / flight in the FAA LADD industry list.
  name: isBlocked
  type: boolean
- description: 'For blocked aircraft only: the date when the aircraft / flight was blocked. Will not be included for blocked dates at or prior to September 15, 2024.'
  name: blockedSince
  type: string
- description: 'For unblocked aircraft only: the date when the aircraft / flight was last blocked. Will not be included for blocked dates at or prior to September 15, 2024 or for the aircraft that were never blocked.'
  name: lastBlockedOn
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-faa-ladd-aircraft-status-contract-schema.json
slug: aerodatabox-faa-ladd-aircraft-status-contract
source_filename: aerodatabox-faa-ladd-aircraft-status-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-faa-ladd-aircraft-status-contract-schema.json\",\n  \"title\": \"FaaLaddAircraftStatusContract\",\n  \"description\": \"Status of the aircraft tail number or callsign in the FAA Limiting Aircraft Data Displayed (LADD) Program list.\\r\\nSee https://www.faa.gov/pilots/ladd for more details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"string\"\n    },\n    \"isBlocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Current status of the aircraft / flight in the FAA LADD industry list.\"\n    },\n    \"blockedSince\": {\n      \"type\": \"string\",\n      \"description\": \"For blocked aircraft only: the date when the aircraft / flight was blocked.\\r\\nWill not be included for blocked dates at or prior to September\
  \ 15, 2024.\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"lastBlockedOn\": {\n      \"type\": \"string\",\n      \"description\": \"For unblocked aircraft only: the date when the aircraft / flight was last blocked.\\r\\nWill not be included for blocked dates at or prior to September 15, 2024 or \\r\\nfor the aircraft that were never blocked.\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"isBlocked\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-faa-ladd-aircraft-status-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FaaLaddAircraftStatusContract
---
