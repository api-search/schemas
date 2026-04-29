---
description: List of shipments for an order
layout: schema
name: ShipmentList
properties_list:
- description: ''
  name: shipments
  type: array
- description: ''
  name: total
  type: integer
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-shipment-list-schema.json
slug: acuity-brands-shipment-list
source_filename: acuity-brands-shipment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-shipment-list-schema.json\",\n  \"title\": \"ShipmentList\",\n  \"description\": \"List of shipments for an order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shipments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Shipment\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-shipment-list-schema.json
tags: []
title: ShipmentList
---
