---
description: ''
layout: schema
name: TriggerCreate
properties_list:
- description: ''
  name: '@type'
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: frequency
  type: string
- description: ''
  name: snapshotTime
  type: string
- description: ''
  name: timezone
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-trigger-create-schema.json
slug: bloomberg-data-license-trigger-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TriggerCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"frequency\": {\n      \"type\": \"string\"\n    },\n    \"snapshotTime\": {\n      \"type\": \"string\"\n    },\n    \"timezone\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-trigger-create-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: TriggerCreate
---
