---
description: ''
layout: schema
name: ShipmentList
properties_list:
- description: ''
  name: shipments
  type: array
- description: Total number of shipments
  name: totalCount
  type: integer
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-shipment-list-schema.json
slug: arcbest-api-shipment-list
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"shipments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"proNumber\": {},\n          \"bolNumber\": {},\n          \"status\": {},\n          \"quoteNumber\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of shipments\",\n      \"example\": 25\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-shipment-list-schema.json\",\n  \"title\": \"ShipmentList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-shipment-list-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: ShipmentList
---
