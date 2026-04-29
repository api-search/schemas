---
description: TransactionLine schema from Avalara API
layout: schema
name: TransactionLine
properties_list:
- description: ''
  name: lineNumber
  type: string
- description: Excise product code
  name: productCode
  type: string
- description: Unit of measure
  name: unitOfMeasure
  type: string
- description: Quantity of product
  name: quantity
  type: number
- description: Line amount
  name: amount
  type: number
- description: ''
  name: origin
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: billOfLadingNumber
  type: string
- description: ''
  name: carrierName
  type: string
- description: ''
  name: modeOfTransport
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-transaction-line-schema.json
slug: excise-transaction-line
source_filename: excise-transaction-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-transaction-line-schema.json\",\n  \"title\": \"TransactionLine\",\n  \"description\": \"TransactionLine schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineNumber\": {\n      \"type\": \"string\"\n    },\n    \"productCode\": {\n      \"type\": \"string\",\n      \"description\": \"Excise product code\"\n    },\n    \"unitOfMeasure\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GAL\",\n        \"LTR\",\n        \"BBL\",\n        \"TON\",\n        \"EA\"\n      ],\n      \"description\": \"Unit of measure\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Quantity of product\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Line\
  \ amount\"\n    },\n    \"origin\": {\n      \"$ref\": \"#/components/schemas/ExciseAddress\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/components/schemas/ExciseAddress\"\n    },\n    \"billOfLadingNumber\": {\n      \"type\": \"string\"\n    },\n    \"carrierName\": {\n      \"type\": \"string\"\n    },\n    \"modeOfTransport\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Truck\",\n        \"Pipeline\",\n        \"Rail\",\n        \"Vessel\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-transaction-line-schema.json
tags:
- Taxes
title: TransactionLine
---
