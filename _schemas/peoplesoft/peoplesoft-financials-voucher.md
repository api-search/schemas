---
description: PeopleSoft AP voucher.
layout: schema
name: Voucher
properties_list:
- description: Business unit.
  name: BUSINESS_UNIT
  type: string
- description: Voucher ID.
  name: VOUCHER_ID
  type: string
- description: Vendor ID.
  name: VENDOR_ID
  type: string
- description: Invoice number.
  name: INVOICE_ID
  type: string
- description: Invoice date.
  name: INVOICE_DT
  type: string
- description: Gross amount.
  name: GROSS_AMT
  type: number
- description: Currency code.
  name: CURRENCY_CD
  type: string
- description: Voucher status.
  name: VCHR_HDR_STATUS
  type: string
- description: Due date.
  name: DUE_DT
  type: string
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-financials-voucher-schema.json
slug: peoplesoft-financials-voucher
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-financials-voucher-schema.json\",\n  \"title\": \"Voucher\",\n  \"description\": \"PeopleSoft AP voucher.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BUSINESS_UNIT\": {\n      \"type\": \"string\",\n      \"description\": \"Business unit.\",\n      \"example\": \"US001\"\n    },\n    \"VOUCHER_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Voucher ID.\",\n      \"example\": \"00045678\"\n    },\n    \"VENDOR_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor ID.\",\n      \"example\": \"VND001234\"\n    },\n    \"INVOICE_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice number.\",\n      \"example\": \"INV-2026-0042\"\n    },\n    \"INVOICE_DT\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\":\
  \ \"Invoice date.\",\n      \"example\": \"2026-04-15\"\n    },\n    \"GROSS_AMT\": {\n      \"type\": \"number\",\n      \"description\": \"Gross amount.\",\n      \"example\": 12500.0\n    },\n    \"CURRENCY_CD\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code.\",\n      \"example\": \"USD\"\n    },\n    \"VCHR_HDR_STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"Voucher status.\",\n      \"enum\": [\n        \"O\",\n        \"A\",\n        \"C\",\n        \"P\",\n        \"V\",\n        \"X\"\n      ],\n      \"example\": \"A\"\n    },\n    \"DUE_DT\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Due date.\",\n      \"example\": \"2026-05-15\"\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-financials-voucher-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: Voucher
---
