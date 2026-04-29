---
description: Request body for inviting a new member
layout: schema
name: InviteMemberRequest
properties_list:
- description: Email address for the new member
  name: email
  type: string
- description: First name of the new member
  name: first_name
  type: string
- description: Last name of the new member
  name: last_name
  type: string
- description: Role to assign to the new member
  name: role
  type: string
- description: Department to assign the new member to
  name: department
  type: string
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-invite-member-request-schema.json
slug: abacus-invite-member-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-invite-member-request-schema.json\",\n  \"title\": \"InviteMemberRequest\",\n  \"description\": \"Request body for inviting a new member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address for the new member\",\n      \"example\": \"newuser@example.com\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the new member\",\n      \"example\": \"John\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the new member\",\n      \"example\": \"Doe\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role to assign to the new member\",\n      \"enum\": [\n        \"employee\",\n        \"manager\",\n   \
  \     \"admin\"\n      ],\n      \"default\": \"employee\",\n      \"example\": \"employee\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department to assign the new member to\",\n      \"example\": \"Engineering\"\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"first_name\",\n    \"last_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-invite-member-request-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: InviteMemberRequest
---
