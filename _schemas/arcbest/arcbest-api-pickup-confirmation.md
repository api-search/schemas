---
description: ''
layout: schema
name: PickupConfirmation
properties_list:
- description: Pickup confirmation number
  name: confirmationNumber
  type: string
- description: Confirmed pickup date
  name: pickupDate
  type: string
- description: Pickup status
  name: status
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-pickup-confirmation-schema.json
slug: arcbest-api-pickup-confirmation
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Pickup confirmation number\",\n      \"example\": \"PU-20260420-001\"\n    },\n    \"pickupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Confirmed pickup date\",\n      \"example\": \"2026-04-20\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Pickup status\",\n      \"enum\": [\n        \"SCHEDULED\",\n        \"CONFIRMED\",\n        \"CANCELLED\"\n      ],\n      \"example\": \"SCHEDULED\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-pickup-confirmation-schema.json\",\n  \"title\": \"PickupConfirmation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-pickup-confirmation-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: PickupConfirmation
---
