---
description: A customer (debtor) tracked in the Debbie platform.
layout: schema
name: Debbie Customer
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: reference_id
  type: string
- description: ''
  name: name
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
- description: ''
  name: country
  type: string
- description: ''
  name: national_id
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Debbie Collect
provider_slug: debbie-collect
schema_file: json-schema/debbie-customer.json
slug: debbie-customer
source_filename: debbie-customer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/debbie-collect/json-schema/debbie-customer.json\",\n  \"title\": \"Debbie Customer\",\n  \"description\": \"A customer (debtor) tracked in the Debbie platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\"},\n    \"reference_id\": {\"type\": \"string\"},\n    \"name\": {\"type\": \"string\"},\n    \"email\": {\"type\": \"string\", \"format\": \"email\"},\n    \"phone\": {\"type\": \"string\"},\n    \"address\": {\"type\": \"object\"},\n    \"country\": {\"type\": \"string\"},\n    \"national_id\": {\"type\": \"string\"},\n    \"created_at\": {\"type\": \"string\", \"format\": \"date-time\"}\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/json-schema/debbie-customer.json
tags:
- Accounts Receivable
- Collections
- Debt Collection
- FinTech
- Payments
- SaaS
title: Debbie Customer
---
