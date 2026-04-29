---
description: BrazilTaxDetail schema from Avalara API
layout: schema
name: BrazilTaxDetail
properties_list:
- description: Brazilian tax type
  name: taxType
  type: string
- description: ''
  name: taxBase
  type: number
- description: ''
  name: taxRate
  type: number
- description: ''
  name: taxAmount
  type: number
- description: ''
  name: exemptAmount
  type: number
- description: ''
  name: cstCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-brazil-tax-detail-schema.json
slug: avatax-brazil-brazil-tax-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-brazil-tax-detail-schema.json\",\n  \"title\": \"BrazilTaxDetail\",\n  \"description\": \"BrazilTaxDetail schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taxType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ICMS\",\n        \"ICMS_ST\",\n        \"IPI\",\n        \"PIS\",\n        \"COFINS\",\n        \"ISS\",\n        \"CSLL\",\n        \"IRRF\",\n        \"INSS\",\n        \"IOF\"\n      ],\n      \"description\": \"Brazilian tax type\"\n    },\n    \"taxBase\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"exemptAmount\": {\n      \"type\":\
  \ \"number\",\n      \"format\": \"double\"\n    },\n    \"cstCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-brazil-tax-detail-schema.json
tags:
- Taxes
title: BrazilTaxDetail
---
