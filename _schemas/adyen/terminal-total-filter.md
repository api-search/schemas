---
description: TotalFilter schema from Adyen API
layout: schema
name: TotalFilter
properties_list:
- description: ''
  name: POIID
  type: string
- description: ''
  name: SaleID
  type: string
- description: ''
  name: OperatorID
  type: string
- description: ''
  name: ShiftNumber
  type: string
- description: ''
  name: TotalsGroupID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-total-filter-schema.json
slug: terminal-total-filter
source_filename: terminal-total-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-total-filter-schema.json\",\n  \"title\": \"TotalFilter\",\n  \"description\": \"TotalFilter schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"POIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"SaleID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"OperatorID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"ShiftNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"TotalsGroupID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,16}$\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-total-filter-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TotalFilter
---
