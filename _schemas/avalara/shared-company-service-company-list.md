---
description: CompanyList schema from Avalara API
layout: schema
name: CompanyList
properties_list:
- description: ''
  name: '@recordSetCount'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/shared-company-service-company-list-schema.json
slug: shared-company-service-company-list
source_filename: shared-company-service-company-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/shared-company-service-company-list-schema.json\",\n  \"title\": \"CompanyList\",\n  \"description\": \"CompanyList schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@recordSetCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SharedCompany\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/shared-company-service-company-list-schema.json
tags:
- Taxes
title: CompanyList
---
