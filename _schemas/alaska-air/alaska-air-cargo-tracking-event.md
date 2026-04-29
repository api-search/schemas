---
description: A cargo tracking event
layout: schema
name: TrackingEvent
properties_list:
- description: Event timestamp
  name: timestamp
  type: string
- description: Location IATA code
  name: location
  type: string
- description: Event type
  name: event
  type: string
- description: Event description
  name: description
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-tracking-event-schema.json
slug: alaska-air-cargo-tracking-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-tracking-event-schema.json\",\n  \"title\": \"TrackingEvent\",\n  \"description\": \"A cargo tracking event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Event timestamp\",\n      \"example\": \"2026-04-20T10:30:00-07:00\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Location IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Event type\",\n      \"example\": \"Accepted\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Event description\",\n      \"example\": \"Shipment accepted at Seattle\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-tracking-event-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: TrackingEvent
---
