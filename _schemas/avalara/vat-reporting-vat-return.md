---
description: VATReturn schema from Avalara API
layout: schema
name: VATReturn
properties_list:
- description: ''
  name: returnId
  type: string
- description: ''
  name: companyId
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ''
  name: vatRegistrationNumber
  type: string
- description: ''
  name: returnType
  type: string
- description: ''
  name: periodStart
  type: string
- description: ''
  name: periodEnd
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: totalOutputVAT
  type: number
- description: ''
  name: totalInputVAT
  type: number
- description: ''
  name: netVATDue
  type: number
- description: ''
  name: submissionDate
  type: string
- description: ''
  name: currency
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-vat-return-schema.json
slug: vat-reporting-vat-return
source_filename: vat-reporting-vat-return-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-vat-return-schema.json\",\n  \"title\": \"VATReturn\",\n  \"description\": \"VATReturn schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"returnId\": {\n      \"type\": \"string\"\n    },\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"vatRegistrationNumber\": {\n      \"type\": \"string\"\n    },\n    \"returnType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"VATReturn\",\n        \"ECListing\",\n        \"Intrastat\"\n      ]\n    },\n    \"periodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"periodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"\
  status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Draft\",\n        \"Submitted\",\n        \"Accepted\",\n        \"Rejected\"\n      ]\n    },\n    \"totalOutputVAT\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"totalInputVAT\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"netVATDue\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"submissionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-vat-return-schema.json
tags:
- Taxes
title: VATReturn
---
