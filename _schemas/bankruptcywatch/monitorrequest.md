---
description: Bankruptcy monitoring request
layout: schema
name: MonitorRequest
properties_list:
- description: Monitor type (debtor, entity, portfolio)
  name: monitorType
  type: string
- description: Search criteria for triggering alerts
  name: criteria
  type: object
- description: ''
  name: notificationEmail
  type: string
- description: ''
  name: webhookUrl
  type: string
- description: ''
  name: label
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/monitorrequest-schema.json
slug: monitorrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/monitorrequest-schema.json\",\n  \"title\": \"MonitorRequest\",\n  \"type\": \"object\",\n  \"description\": \"Bankruptcy monitoring request\",\n  \"required\": [\n    \"monitorType\",\n    \"criteria\"\n  ],\n  \"properties\": {\n    \"monitorType\": {\n      \"type\": \"string\",\n      \"description\": \"Monitor type (debtor, entity, portfolio)\"\n    },\n    \"criteria\": {\n      \"type\": \"object\",\n      \"description\": \"Search criteria for triggering alerts\"\n    },\n    \"notificationEmail\": {\n      \"type\": \"string\"\n    },\n    \"webhookUrl\": {\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/monitorrequest-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: MonitorRequest
---
