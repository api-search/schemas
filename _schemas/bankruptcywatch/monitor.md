---
description: A bankruptcy monitoring alert
layout: schema
name: Monitor
properties_list:
- description: ''
  name: monitorId
  type: string
- description: ''
  name: monitorType
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: lastTriggeredAt
  type: string
- description: ''
  name: alertCount
  type: integer
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/monitor-schema.json
slug: monitor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/monitor-schema.json\",\n  \"title\": \"Monitor\",\n  \"type\": \"object\",\n  \"description\": \"A bankruptcy monitoring alert\",\n  \"properties\": {\n    \"monitorId\": {\n      \"type\": \"string\"\n    },\n    \"monitorType\": {\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"paused\",\n        \"deleted\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastTriggeredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"alertCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/monitor-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: Monitor
---
