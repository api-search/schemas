---
description: ''
layout: schema
name: ShipmentRequest
properties_list:
- description: Rate quote number to use for booking
  name: quoteNumber
  type: string
- description: ''
  name: shipper
  type: object
- description: ''
  name: consignee
  type: object
- description: ''
  name: items
  type: array
- description: Customer reference number
  name: referenceNumber
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-shipment-request-schema.json
slug: arcbest-api-shipment-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"shipper\",\n    \"consignee\"\n  ],\n  \"properties\": {\n    \"quoteNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Rate quote number to use for booking\",\n      \"example\": \"Q-20260419-001\"\n    },\n    \"shipper\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Company or person name\",\n          \"example\": \"ACME Corp\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address\",\n          \"example\": \"123 Main St\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City\",\n          \"example\": \"Benton\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State abbreviation\",\n          \"example\": \"AR\"\n        },\n        \"zip\": {\n          \"\
  type\": \"string\",\n          \"description\": \"ZIP code\",\n          \"example\": \"72015\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"example\": \"US\"\n        }\n      }\n    },\n    \"consignee\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Company or person name\",\n          \"example\": \"ACME Corp\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address\",\n          \"example\": \"123 Main St\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City\",\n          \"example\": \"Benton\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State abbreviation\",\n          \"example\": \"AR\"\n        },\n        \"zip\": {\n     \
  \     \"type\": \"string\",\n          \"description\": \"ZIP code\",\n          \"example\": \"72015\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"example\": \"US\"\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"weight\": {},\n          \"freightClass\": {},\n          \"pieces\": {},\n          \"description\": {},\n          \"length\": {},\n          \"width\": {},\n          \"height\": {}\n        }\n      }\n    },\n    \"referenceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Customer reference number\",\n      \"example\": \"PO-98765\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-shipment-request-schema.json\"\
  ,\n  \"title\": \"ShipmentRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-shipment-request-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: ShipmentRequest
---
