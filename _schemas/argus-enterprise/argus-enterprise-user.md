---
description: User schema from ARGUS Enterprise API
layout: schema
name: User
properties_list:
- description: Unique user identifier
  name: id
  type: string
- description: Username
  name: username
  type: string
- description: User email address
  name: email
  type: string
- description: First name
  name: firstName
  type: string
- description: Last name
  name: lastName
  type: string
- description: User role
  name: role
  type: string
- description: Last login timestamp
  name: lastLogin
  type: string
- description: Whether the user account is active
  name: active
  type: boolean
- description: ''
  name: createdAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-user-schema.json
slug: argus-enterprise-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"User schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique user identifier\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Admin\",\n  \
  \      \"Analyst\",\n        \"Viewer\"\n      ],\n      \"description\": \"User role\"\n    },\n    \"lastLogin\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last login timestamp\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-user-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: User
---
