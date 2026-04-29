---
description: Pagination schema from Amdocs API
layout: schema
name: Pagination
properties_list:
- description: ''
  name: page
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: totalPages
  type: integer
- description: ''
  name: totalItems
  type: integer
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-pagination-schema.json
slug: connectx-pagination
source_filename: connectx-pagination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-pagination-schema.json\",\n  \"title\": \"Pagination\",\n  \"description\": \"Pagination schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\"\n    },\n    \"totalItems\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-pagination-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: Pagination
---
