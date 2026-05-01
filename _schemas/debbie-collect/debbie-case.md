---
description: A debt-collection case in the Debbie platform.
layout: schema
name: Debbie Case
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: creditor_id
  type: string
- description: ''
  name: customer_id
  type: string
- description: ''
  name: reference_id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: principal_amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: outstanding_amount
  type: number
- description: ''
  name: due_date
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Debbie Collect
provider_slug: debbie-collect
schema_file: json-schema/debbie-case.json
slug: debbie-case
source_filename: debbie-case.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/debbie-collect/json-schema/debbie-case.json\",\n  \"title\": \"Debbie Case\",\n  \"description\": \"A debt-collection case in the Debbie platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\"},\n    \"creditor_id\": {\"type\": \"string\"},\n    \"customer_id\": {\"type\": \"string\"},\n    \"reference_id\": {\"type\": \"string\"},\n    \"status\": {\"type\": \"string\", \"enum\": [\"open\", \"in_progress\", \"settled\", \"closed\", \"legal\", \"cancelled\"]},\n    \"principal_amount\": {\"type\": \"number\"},\n    \"currency\": {\"type\": \"string\"},\n    \"outstanding_amount\": {\"type\": \"number\"},\n    \"due_date\": {\"type\": \"string\", \"format\": \"date\"},\n    \"created_at\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"updated_at\": {\"type\": \"string\", \"format\": \"date-time\"}\n  },\n  \"required\"\
  : [\"id\", \"creditor_id\", \"customer_id\", \"principal_amount\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/json-schema/debbie-case.json
tags:
- Accounts Receivable
- Collections
- Debt Collection
- FinTech
- Payments
- SaaS
title: Debbie Case
---
