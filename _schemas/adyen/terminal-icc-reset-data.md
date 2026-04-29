---
description: ICCResetData schema from Adyen API
layout: schema
name: ICCResetData
properties_list:
- description: ''
  name: ATRValue
  type: string
- description: ''
  name: CardStatusWords
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-icc-reset-data-schema.json
slug: terminal-icc-reset-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-icc-reset-data-schema.json\",\n  \"title\": \"ICCResetData\",\n  \"description\": \"ICCResetData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ATRValue\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{1,100}$\"\n    },\n    \"CardStatusWords\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{2,2}$\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-icc-reset-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ICCResetData
---
