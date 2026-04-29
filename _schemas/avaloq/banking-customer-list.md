---
description: Paginated list of customers
layout: schema
name: CustomerList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-customer-list-schema.json
slug: banking-customer-list
source_filename: banking-customer-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-customer-list-schema.json\",\n  \"title\": \"CustomerList\",\n  \"description\": \"Paginated list of customers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Customer\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 1250\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-customer-list-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: CustomerList
---
