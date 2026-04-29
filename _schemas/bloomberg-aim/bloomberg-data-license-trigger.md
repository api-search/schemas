---
description: ''
layout: schema
name: Trigger
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
  name: description
  type: string
- description: ''
  name: frequency
  type: string
- description: Time of day for the snapshot (HH:MM)
  name: snapshotTime
  type: string
- description: Timezone for the trigger schedule
  name: timezone
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-trigger-schema.json
slug: bloomberg-data-license-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Trigger\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"frequency\": {\n      \"type\": \"string\"\n    },\n    \"snapshotTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time of day for the snapshot (HH:MM)\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for the trigger schedule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-trigger-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Trigger
---
