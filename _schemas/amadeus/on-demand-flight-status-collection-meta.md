---
description: ''
layout: schema
name: Collection_Meta
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-collection-meta-schema.json
slug: on-demand-flight-status-collection-meta
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Collection_Meta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"previous\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"first\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"up\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-collection-meta-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: Collection_Meta
---
