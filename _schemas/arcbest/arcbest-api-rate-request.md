---
description: ''
layout: schema
name: RateRequest
properties_list:
- description: ''
  name: origin
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: items
  type: array
- description: Requested service type
  name: serviceType
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-rate-request-schema.json
slug: arcbest-api-rate-request
source_filename: arcbest-api-rate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"origin\",\n    \"destination\",\n    \"items\"\n  ],\n  \"properties\": {\n    \"origin\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Company or person name\",\n          \"example\": \"ACME Corp\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address\",\n          \"example\": \"123 Main St\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City\",\n          \"example\": \"Benton\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State abbreviation\",\n          \"example\": \"AR\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"ZIP code\",\n          \"example\": \"72015\"\n        },\n        \"country\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"example\": \"US\"\n        }\n      }\n    },\n    \"destination\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Company or person name\",\n          \"example\": \"ACME Corp\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address\",\n          \"example\": \"123 Main St\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City\",\n          \"example\": \"Benton\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State abbreviation\",\n          \"example\": \"AR\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"ZIP code\",\n          \"example\": \"72015\"\n        },\n        \"country\": {\n         \
  \ \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"example\": \"US\"\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"weight\": {},\n          \"freightClass\": {},\n          \"pieces\": {},\n          \"description\": {},\n          \"length\": {},\n          \"width\": {},\n          \"height\": {}\n        }\n      }\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Requested service type\",\n      \"enum\": [\n        \"STANDARD\",\n        \"EXPEDITED\",\n        \"GUARANTEED\"\n      ],\n      \"example\": \"STANDARD\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-rate-request-schema.json\",\n  \"title\": \"RateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-rate-request-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: RateRequest
---
