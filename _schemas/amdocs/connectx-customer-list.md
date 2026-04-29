---
description: CustomerList schema from Amdocs API
layout: schema
name: CustomerList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-customer-list-schema.json
slug: connectx-customer-list
source_filename: connectx-customer-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-list-schema.json\",\n  \"title\": \"CustomerList\",\n  \"description\": \"CustomerList schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Customer\"\n      }\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-list-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: CustomerList
---
