---
description: An organization member with expense management access
layout: schema
name: Member
properties_list:
- description: Unique member identifier
  name: id
  type: string
- description: Member email address
  name: email
  type: string
- description: Member first name
  name: first_name
  type: string
- description: Member last name
  name: last_name
  type: string
- description: Current member status
  name: status
  type: string
- description: Member role in the organization
  name: role
  type: string
- description: Department the member belongs to
  name: department
  type: string
- description: Timestamp when the member was created
  name: created_at
  type: string
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-member-schema.json
slug: abacus-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"An organization member with expense management access\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique member identifier\",\n      \"example\": \"500123\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Member email address\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Member first name\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Member last name\",\n      \"example\": \"Smith\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current member\
  \ status\",\n      \"enum\": [\n        \"active\",\n        \"invited\",\n        \"suspended\"\n      ],\n      \"example\": \"active\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Member role in the organization\",\n      \"enum\": [\n        \"employee\",\n        \"manager\",\n        \"admin\"\n      ],\n      \"example\": \"employee\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department the member belongs to\",\n      \"example\": \"Engineering\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the member was created\",\n      \"example\": \"2025-01-15T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-member-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: Member
---
