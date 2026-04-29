---
description: ''
layout: schema
name: FreightItem
properties_list:
- description: Weight in pounds
  name: weight
  type: number
- description: NMFC freight classification
  name: freightClass
  type: string
- description: Number of pieces
  name: pieces
  type: integer
- description: Commodity description
  name: description
  type: string
- description: Length in inches
  name: length
  type: number
- description: Width in inches
  name: width
  type: number
- description: Height in inches
  name: height
  type: number
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-freight-item-schema.json
slug: arcbest-api-freight-item
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Weight in pounds\",\n      \"example\": 500\n    },\n    \"freightClass\": {\n      \"type\": \"string\",\n      \"description\": \"NMFC freight classification\",\n      \"example\": \"70\"\n    },\n    \"pieces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pieces\",\n      \"example\": 2\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity description\",\n      \"example\": \"Machine parts\"\n    },\n    \"length\": {\n      \"type\": \"number\",\n      \"description\": \"Length in inches\",\n      \"example\": 48.0\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Width in inches\",\n      \"example\": 40.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Height in inches\",\n      \"example\": 36.0\n    }\n  },\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-freight-item-schema.json\",\n  \"title\": \"FreightItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-freight-item-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: FreightItem
---
