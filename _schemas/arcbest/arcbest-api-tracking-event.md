---
description: ''
layout: schema
name: TrackingEvent
properties_list:
- description: Event timestamp
  name: date
  type: string
- description: Event description
  name: description
  type: string
- description: Event location
  name: location
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-tracking-event-schema.json
slug: arcbest-api-tracking-event
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Event timestamp\",\n      \"example\": \"2026-04-19T08:00:00Z\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Event description\",\n      \"example\": \"Shipment picked up\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Event location\",\n      \"example\": \"Benton, AR\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-tracking-event-schema.json\",\n  \"title\": \"TrackingEvent\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-tracking-event-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: TrackingEvent
---
