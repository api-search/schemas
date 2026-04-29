---
description: AmountsResp schema from Adyen API
layout: schema
name: AmountsResp
properties_list:
- description: ''
  name: Currency
  type: string
- description: ''
  name: AuthorizedAmount
  type: number
- description: ''
  name: TotalRebatesAmount
  type: number
- description: ''
  name: TotalFeesAmount
  type: number
- description: ''
  name: CashBackAmount
  type: number
- description: ''
  name: TipAmount
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-amounts-resp-schema.json
slug: terminal-amounts-resp
source_filename: terminal-amounts-resp-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-amounts-resp-schema.json\",\n  \"title\": \"AmountsResp\",\n  \"description\": \"AmountsResp schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    },\n    \"AuthorizedAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"TotalRebatesAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"TotalFeesAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"CashBackAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"TipAmount\": {\n      \"type\": \"number\",\n   \
  \   \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\n    \"AuthorizedAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-amounts-resp-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AmountsResp
---
