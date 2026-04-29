---
description: TaxResult schema from Avalara API
layout: schema
name: TaxResult
properties_list:
- description: Billable flag
  name: bill
  type: boolean
- description: Compliance flag
  name: cmpl
  type: boolean
- description: Taxable measure
  name: tm
  type: number
- description: Calculation type
  name: calc
  type: integer
- description: Tax category
  name: cat
  type: string
- description: Category ID
  name: cid
  type: integer
- description: Tax name
  name: name
  type: string
- description: Exempt amount
  name: exm
  type: number
- description: Lines
  name: lns
  type: integer
- description: Minutes
  name: min
  type: number
- description: PCode
  name: pcd
  type: integer
- description: Tax rate
  name: rate
  type: number
- description: Surcharge flag
  name: sur
  type: boolean
- description: Tax amount
  name: tax
  type: number
- description: Tax level (Federal, State, County, Local)
  name: lvl
  type: integer
- description: Tax type ID
  name: tid
  type: integer
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-tax-result-schema.json
slug: communications-tax-result
source_filename: communications-tax-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-tax-result-schema.json\",\n  \"title\": \"TaxResult\",\n  \"description\": \"TaxResult schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bill\": {\n      \"type\": \"boolean\",\n      \"description\": \"Billable flag\"\n    },\n    \"cmpl\": {\n      \"type\": \"boolean\",\n      \"description\": \"Compliance flag\"\n    },\n    \"tm\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Taxable measure\"\n    },\n    \"calc\": {\n      \"type\": \"integer\",\n      \"description\": \"Calculation type\"\n    },\n    \"cat\": {\n      \"type\": \"string\",\n      \"description\": \"Tax category\"\n    },\n    \"cid\": {\n      \"type\": \"integer\",\n      \"description\": \"Category ID\"\n    },\n    \"name\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Tax name\"\n    },\n    \"exm\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Exempt amount\"\n    },\n    \"lns\": {\n      \"type\": \"integer\",\n      \"description\": \"Lines\"\n    },\n    \"min\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Minutes\"\n    },\n    \"pcd\": {\n      \"type\": \"integer\",\n      \"description\": \"PCode\"\n    },\n    \"rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Tax rate\"\n    },\n    \"sur\": {\n      \"type\": \"boolean\",\n      \"description\": \"Surcharge flag\"\n    },\n    \"tax\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Tax amount\"\n    },\n    \"lvl\": {\n      \"type\": \"integer\",\n      \"description\": \"Tax level (Federal, State, County, Local)\"\n    },\n    \"tid\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Tax type ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-tax-result-schema.json
tags:
- Taxes
title: TaxResult
---
