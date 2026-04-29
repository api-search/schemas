---
description: Subscription schema from Amdocs API
layout: schema
name: Subscription
properties_list:
- description: ''
  name: subscriptionId
  type: string
- description: ''
  name: customerId
  type: string
- description: ''
  name: productId
  type: string
- description: ''
  name: productName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: monthlyCharge
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: addons
  type: array
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-subscription-schema.json
slug: connectx-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-subscription-schema.json\",\n  \"title\": \"Subscription\",\n  \"description\": \"Subscription schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscriptionId\": {\n      \"type\": \"string\"\n    },\n    \"customerId\": {\n      \"type\": \"string\"\n    },\n    \"productId\": {\n      \"type\": \"string\"\n    },\n    \"productName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Suspended\",\n        \"Cancelled\",\n        \"Pending\"\n      ]\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"monthlyCharge\": {\n      \"type\": \"number\"\n    },\n\
  \    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\"\n    },\n    \"addons\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"addonId\": {\n            \"type\": \"string\"\n          },\n          \"addonName\": {\n            \"type\": \"string\"\n          },\n          \"charge\": {\n            \"type\": \"number\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-subscription-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: Subscription
---
