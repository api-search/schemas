---
description: ''
layout: schema
name: TrackingStatus
properties_list:
- description: PRO number
  name: proNumber
  type: string
- description: Current shipment status
  name: status
  type: string
- description: Last known location
  name: lastLocation
  type: string
- description: Estimated delivery date
  name: estimatedDelivery
  type: string
- description: ''
  name: events
  type: array
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-tracking-status-schema.json
slug: arcbest-api-tracking-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"proNumber\": {\n      \"type\": \"string\",\n      \"description\": \"PRO number\",\n      \"example\": \"PRO-123456789\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current shipment status\",\n      \"enum\": [\n        \"BOOKED\",\n        \"PICKED_UP\",\n        \"IN_TRANSIT\",\n        \"OUT_FOR_DELIVERY\",\n        \"DELIVERED\",\n        \"EXCEPTION\"\n      ],\n      \"example\": \"IN_TRANSIT\"\n    },\n    \"lastLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Last known location\",\n      \"example\": \"Kansas City, MO\"\n    },\n    \"estimatedDelivery\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated delivery date\",\n      \"example\": \"2026-04-22\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"date\": {},\n\
  \          \"description\": {},\n          \"location\": {}\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-tracking-status-schema.json\",\n  \"title\": \"TrackingStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-tracking-status-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: TrackingStatus
---
