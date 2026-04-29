---
description: CustomerUpdate schema from Amdocs API
layout: schema
name: CustomerUpdate
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: address
  type: object
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-customer-update-schema.json
slug: connectx-customer-update
source_filename: connectx-customer-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-update-schema.json\",\n  \"title\": \"CustomerUpdate\",\n  \"description\": \"CustomerUpdate schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Inactive\",\n        \"Suspended\"\n      ]\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-update-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: CustomerUpdate
---
