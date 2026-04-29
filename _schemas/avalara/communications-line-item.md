---
description: LineItem schema from Avalara API
layout: schema
name: LineItem
properties_list:
- description: Line item reference
  name: ref
  type: string
- description: ''
  name: from
  type: object
- description: ''
  name: to
  type: object
- description: Charge amount
  name: chg
  type: number
- description: Number of lines
  name: line
  type: integer
- description: Number of locations
  name: loc
  type: integer
- description: Minutes
  name: min
  type: number
- description: Sale type (0=Wholesale, 1=Retail, 2=Consumed)
  name: sale
  type: integer
- description: Transaction type
  name: tran
  type: integer
- description: Service type
  name: serv
  type: integer
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-line-item-schema.json
slug: communications-line-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-line-item-schema.json\",\n  \"title\": \"LineItem\",\n  \"description\": \"LineItem schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"Line item reference\"\n    },\n    \"from\": {\n      \"$ref\": \"#/components/schemas/Location\"\n    },\n    \"to\": {\n      \"$ref\": \"#/components/schemas/Location\"\n    },\n    \"chg\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Charge amount\"\n    },\n    \"line\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of lines\"\n    },\n    \"loc\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of locations\"\n    },\n    \"min\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\
  ,\n      \"description\": \"Minutes\"\n    },\n    \"sale\": {\n      \"type\": \"integer\",\n      \"description\": \"Sale type (0=Wholesale, 1=Retail, 2=Consumed)\"\n    },\n    \"tran\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction type\"\n    },\n    \"serv\": {\n      \"type\": \"integer\",\n      \"description\": \"Service type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-line-item-schema.json
tags:
- Taxes
title: LineItem
---
