---
description: Acronis tenant representing a company, partner, or customer account
layout: schema
name: Tenant
properties_list:
- description: Tenant unique identifier
  name: id
  type: string
- description: Tenant display name
  name: name
  type: string
- description: Tenant type in the hierarchy
  name: kind
  type: string
- description: Whether the tenant is active
  name: enabled
  type: boolean
- description: Parent tenant UUID
  name: parent_id
  type: string
- description: Customer account type
  name: customer_type
  type: string
- description: Tenant creation timestamp
  name: created_at
  type: string
- description: Last update timestamp
  name: updated_at
  type: string
- description: Optimistic concurrency version
  name: version
  type: integer
- description: ''
  name: contact
  type: object
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-tenant-schema.json
slug: account-management-tenant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-tenant-schema.json\",\n  \"title\": \"Tenant\",\n  \"description\": \"Acronis tenant representing a company, partner, or customer account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Tenant unique identifier\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant display name\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"root\",\n        \"partner\",\n        \"folder\",\n        \"customer\",\n        \"unit\"\n      ],\n      \"description\": \"Tenant type in the hierarchy\",\n      \"example\": \"customer\"\n    },\n\
  \    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the tenant is active\",\n      \"example\": true\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Parent tenant UUID\"\n    },\n    \"customer_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"default\",\n        \"trial\"\n      ],\n      \"description\": \"Customer account type\",\n      \"example\": \"default\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Tenant creation timestamp\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Optimistic concurrency version\",\n      \"example\": 1\n    },\n    \"contact\": {\n      \"\
  $ref\": \"#/components/schemas/Contact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-tenant-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Tenant
---
