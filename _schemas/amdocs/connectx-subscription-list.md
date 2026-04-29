---
description: SubscriptionList schema from Amdocs API
layout: schema
name: SubscriptionList
properties_list:
- description: ''
  name: data
  type: array
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-subscription-list-schema.json
slug: connectx-subscription-list
source_filename: connectx-subscription-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-subscription-list-schema.json\",\n  \"title\": \"SubscriptionList\",\n  \"description\": \"SubscriptionList schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Subscription\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-subscription-list-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: SubscriptionList
---
