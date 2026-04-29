---
description: ''
layout: schema
name: TimeOffBalance
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The current balance.
  name: balance
  type: number
- description: The unit of the balance (e.g., Hours, Days).
  name: unit
  type: string
- description: The effective date of the balance.
  name: asOfDate
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/absenceManagement-time-off-balance-schema.json
slug: absenceManagement-time-off-balance
source_filename: absenceManagement-time-off-balance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeOffBalance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"The current balance.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of the balance (e.g., Hours, Days).\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"description\": \"The effective date of the balance.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/absenceManagement-time-off-balance-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeOffBalance
---
