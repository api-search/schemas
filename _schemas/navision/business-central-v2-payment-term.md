---
description: ''
layout: schema
name: PaymentTerm
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: displayName
  type: string
- description: The date formula for due date calculation
  name: dueDateCalculation
  type: string
- description: The date formula for discount date calculation
  name: discountDateCalculation
  type: string
- description: ''
  name: discountPercent
  type: number
- description: ''
  name: calculateDiscountOnCreditMemos
  type: boolean
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-payment-term-schema.json
slug: business-central-v2-payment-term
source_filename: business-central-v2-payment-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentTerm\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"dueDateCalculation\": {\n      \"type\": \"string\",\n      \"description\": \"The date formula for due date calculation\"\n    },\n    \"discountDateCalculation\": {\n      \"type\": \"string\",\n      \"description\": \"The date formula for discount date calculation\"\n    },\n    \"discountPercent\": {\n      \"type\": \"number\"\n    },\n    \"calculateDiscountOnCreditMemos\": {\n      \"type\": \"boolean\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-payment-term-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: PaymentTerm
---
