---
description: ProductList schema from Amdocs API
layout: schema
name: ProductList
properties_list:
- description: ''
  name: data
  type: array
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-product-list-schema.json
slug: connectx-product-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-product-list-schema.json\",\n  \"title\": \"ProductList\",\n  \"description\": \"ProductList schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Product\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-product-list-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: ProductList
---
