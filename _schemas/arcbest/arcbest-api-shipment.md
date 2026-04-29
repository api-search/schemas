---
description: ''
layout: schema
name: Shipment
properties_list:
- description: ArcBest PRO (shipment) number
  name: proNumber
  type: string
- description: Bill of Lading number
  name: bolNumber
  type: string
- description: Shipment status
  name: status
  type: string
- description: Rate quote number used for booking
  name: quoteNumber
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-shipment-schema.json
slug: arcbest-api-shipment
source_filename: arcbest-api-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"proNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ArcBest PRO (shipment) number\",\n      \"example\": \"PRO-123456789\"\n    },\n    \"bolNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Bill of Lading number\",\n      \"example\": \"BOL-20260419-001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Shipment status\",\n      \"enum\": [\n        \"BOOKED\",\n        \"PICKED_UP\",\n        \"IN_TRANSIT\",\n        \"OUT_FOR_DELIVERY\",\n        \"DELIVERED\",\n        \"EXCEPTION\"\n      ],\n      \"example\": \"BOOKED\"\n    },\n    \"quoteNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Rate quote number used for booking\",\n      \"example\": \"Q-20260419-001\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-shipment-schema.json\"\
  ,\n  \"title\": \"Shipment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-shipment-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: Shipment
---
