---
description: ''
layout: schema
name: IncomeVerification
properties_list:
- description: ''
  name: userId
  type: string
- description: ''
  name: summary
  type: object
- description: ''
  name: incomeStreams
  type: array
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/incomeverification.json
slug: incomeverification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/incomeverification.json\",\n  \"title\": \"IncomeVerification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"regular\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"monthly\": {\n              \"type\": \"number\"\n            },\n            \"annual\": {\n              \"type\": \"number\"\n            }\n          }\n        },\n        \"irregular\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"monthly\": {\n              \"type\": \"number\"\n            }\n          }\n        }\n      }\n    },\n    \"incomeStreams\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n\
  \        \"properties\": {\n          \"source\": {\n            \"type\": \"string\"\n          },\n          \"amount\": {\n            \"type\": \"number\"\n          },\n          \"frequency\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/incomeverification.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: IncomeVerification
---
