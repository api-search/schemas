---
description: Feed service status contract. Read https://aerodatabox.com/data-coverage for context.
layout: schema
name: FeedServiceStatusContract
properties_list:
- description: ''
  name: service
  type: object
- description: ''
  name: status
  type: object
- description: Date of the oldest flight stored (based on scheduled local times)
  name: minAvailableLocalDate
  type: string
- description: Date of the most recent flight stored (based on scheduled local times)
  name: maxAvailableLocalDate
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-feed-service-status-contract-schema.json
slug: aerodatabox-feed-service-status-contract
source_filename: aerodatabox-feed-service-status-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-feed-service-status-contract-schema.json\",\n  \"title\": \"FeedServiceStatusContract\",\n  \"description\": \"Feed service status contract.\\r\\nRead https://aerodatabox.com/data-coverage for context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service\": {\n      \"$ref\": \"#/components/schemas/FeedServiceEnum\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/FeedServiceStatus\"\n    },\n    \"minAvailableLocalDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the oldest flight stored (based on scheduled local times)\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"deprecated\": true\n    },\n    \"maxAvailableLocalDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the most recent flight stored\
  \ (based on scheduled local times)\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"deprecated\": true\n    }\n  },\n  \"required\": [\n    \"service\",\n    \"status\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-feed-service-status-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FeedServiceStatusContract
---
