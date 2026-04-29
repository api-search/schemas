---
description: Amounts of a payment
layout: schema
name: AmountsReq
properties_list:
- description: ''
  name: Currency
  type: string
- description: ''
  name: RequestedAmount
  type: number
- description: ''
  name: CashBackAmount
  type: number
- description: ''
  name: TipAmount
  type: number
- description: ''
  name: PaidAmount
  type: number
- description: ''
  name: MinimumAmountToDeliver
  type: number
- description: ''
  name: MaximumCashBackAmount
  type: number
- description: ''
  name: MinimumSplitAmount
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-amounts-req-schema.json
slug: terminal-amounts-req
source_filename: terminal-amounts-req-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-amounts-req-schema.json\",\n  \"title\": \"AmountsReq\",\n  \"description\": \"Amounts of a payment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    },\n    \"RequestedAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"CashBackAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"TipAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"PaidAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"MinimumAmountToDeliver\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n\
  \      \"minimum\": 0\n    },\n    \"MaximumCashBackAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"MinimumSplitAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\n    \"Currency\",\n    \"RequestedAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-amounts-req-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AmountsReq
---
