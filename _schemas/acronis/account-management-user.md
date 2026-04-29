---
description: Acronis platform user account
layout: schema
name: User
properties_list:
- description: User unique identifier
  name: id
  type: string
- description: Username/login for the user
  name: login
  type: string
- description: User email address
  name: email
  type: string
- description: ''
  name: firstname
  type: string
- description: ''
  name: lastname
  type: string
- description: Whether the user account is active
  name: enabled
  type: boolean
- description: Tenant the user belongs to
  name: tenant_id
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-user-schema.json
slug: account-management-user
source_filename: account-management-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"Acronis platform user account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User unique identifier\"\n    },\n    \"login\": {\n      \"type\": \"string\",\n      \"description\": \"Username/login for the user\",\n      \"example\": \"jsmith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"firstname\": {\n      \"type\": \"string\",\n      \"example\": \"John\"\n    },\n    \"lastname\": {\n      \"type\": \"string\",\n      \"example\": \"Smith\"\n    },\n    \"enabled\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Whether the user account is active\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Tenant the user belongs to\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-user-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: User
---
