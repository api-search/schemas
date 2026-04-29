---
description: SubscriptionRequest schema from Amdocs API
layout: schema
name: SubscriptionRequest
properties_list:
- description: ''
  name: productId
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: addons
  type: array
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-subscription-request-schema.json
slug: connectx-subscription-request
source_filename: connectx-subscription-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-subscription-request-schema.json\",\n  \"title\": \"SubscriptionRequest\",\n  \"description\": \"SubscriptionRequest schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"addons\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"productId\",\n    \"startDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-subscription-request-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: SubscriptionRequest
---
