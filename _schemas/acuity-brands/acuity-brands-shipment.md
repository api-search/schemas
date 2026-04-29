---
description: Shipment record for an order
layout: schema
name: Shipment
properties_list:
- description: Shipment identifier
  name: shipmentId
  type: string
- description: Associated order ID
  name: orderId
  type: string
- description: Shipping carrier name
  name: carrier
  type: string
- description: Carrier PRO/tracking number
  name: proNumber
  type: string
- description: Carrier tracking URL
  name: trackingUrl
  type: string
- description: ''
  name: shipDate
  type: string
- description: ''
  name: estimatedDeliveryDate
  type: string
- description: Shipment weight in lbs
  name: weight
  type: number
- description: Line items in this shipment
  name: lineItems
  type: array
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-shipment-schema.json
slug: acuity-brands-shipment
source_filename: acuity-brands-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-shipment-schema.json\",\n  \"title\": \"Shipment\",\n  \"description\": \"Shipment record for an order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shipmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Shipment identifier\",\n      \"example\": \"SHP-001\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated order ID\",\n      \"example\": \"ACB-2026-001234\"\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping carrier name\",\n      \"example\": \"UPS Freight\"\n    },\n    \"proNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier PRO/tracking number\",\n      \"example\": \"1Z999AA10123456784\"\n    },\n    \"trackingUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier tracking URL\",\n    \
  \  \"example\": \"https://www.ups.com/track?tracknum=1Z999AA10123456784\"\n    },\n    \"shipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"estimatedDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2026-04-22\"\n    },\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Shipment weight in lbs\",\n      \"example\": 45.5\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"Line items in this shipment\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"lineNumber\": {\n            \"type\": \"integer\",\n            \"example\": 1\n          },\n          \"productNumber\": {\n            \"type\": \"string\",\n            \"example\": \"LBL4 48L ADP\"\n          },\n          \"quantityShipped\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n\
  \        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-shipment-schema.json
tags: []
title: Shipment
---
