---
description: ExciseTaxDetail schema from Avalara API
layout: schema
name: ExciseTaxDetail
properties_list:
- description: Type of excise tax
  name: taxType
  type: string
- description: Taxing jurisdiction
  name: jurisdiction
  type: string
- description: ''
  name: taxRate
  type: number
- description: ''
  name: taxAmount
  type: number
- description: ''
  name: taxableAmount
  type: number
- description: ''
  name: exemptAmount
  type: number
- description: ''
  name: rateType
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-excise-tax-detail-schema.json
slug: excise-excise-tax-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-tax-detail-schema.json\",\n  \"title\": \"ExciseTaxDetail\",\n  \"description\": \"ExciseTaxDetail schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taxType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of excise tax\"\n    },\n    \"jurisdiction\": {\n      \"type\": \"string\",\n      \"description\": \"Taxing jurisdiction\"\n    },\n    \"taxRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxableAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"exemptAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"rateType\": {\n      \"type\": \"string\",\n      \"\
  enum\": [\n        \"PerUnit\",\n        \"Percentage\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-tax-detail-schema.json
tags:
- Taxes
title: ExciseTaxDetail
---
