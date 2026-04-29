---
description: ''
layout: schema
name: PickupRequest
properties_list:
- description: PRO number for the shipment
  name: proNumber
  type: string
- description: Requested pickup date
  name: pickupDate
  type: string
- description: Time freight will be ready (HH:MM)
  name: readyTime
  type: string
- description: Facility closing time (HH:MM)
  name: closeTime
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-pickup-request-schema.json
slug: arcbest-api-pickup-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"proNumber\",\n    \"pickupDate\"\n  ],\n  \"properties\": {\n    \"proNumber\": {\n      \"type\": \"string\",\n      \"description\": \"PRO number for the shipment\",\n      \"example\": \"PRO-123456789\"\n    },\n    \"pickupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested pickup date\",\n      \"example\": \"2026-04-20\"\n    },\n    \"readyTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time freight will be ready (HH:MM)\",\n      \"example\": \"09:00\"\n    },\n    \"closeTime\": {\n      \"type\": \"string\",\n      \"description\": \"Facility closing time (HH:MM)\",\n      \"example\": \"17:00\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-pickup-request-schema.json\",\n  \"title\": \"PickupRequest\"\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-pickup-request-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: PickupRequest
---
