---
description: Request body for updating an existing member
layout: schema
name: UpdateMemberRequest
properties_list:
- description: New role for the member
  name: role
  type: string
- description: New department for the member
  name: department
  type: string
- description: New status for the member
  name: status
  type: string
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-update-member-request-schema.json
slug: abacus-update-member-request
source_filename: abacus-update-member-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-update-member-request-schema.json\",\n  \"title\": \"UpdateMemberRequest\",\n  \"description\": \"Request body for updating an existing member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"New role for the member\",\n      \"enum\": [\n        \"employee\",\n        \"manager\",\n        \"admin\"\n      ],\n      \"example\": \"manager\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"New department for the member\",\n      \"example\": \"Engineering\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"New status for the member\",\n      \"enum\": [\n        \"active\",\n        \"suspended\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-update-member-request-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: UpdateMemberRequest
---
