---
description: Paginated list of members
layout: schema
name: MemberListResponse
properties_list:
- description: ''
  name: members
  type: array
- description: Total number of members
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of results per page
  name: per_page
  type: integer
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-member-list-response-schema.json
slug: abacus-member-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-member-list-response-schema.json\",\n  \"title\": \"MemberListResponse\",\n  \"description\": \"Paginated list of members\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"members\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Member\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of members\",\n      \"example\": 125\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\",\n      \"example\": 1\n    },\n    \"per_page\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results per page\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-member-list-response-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: MemberListResponse
---
