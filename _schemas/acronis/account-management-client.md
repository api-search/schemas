---
description: OAuth2 client credential
layout: schema
name: Client
properties_list:
- description: OAuth2 client identifier
  name: client_id
  type: string
- description: OAuth2 client secret (only shown on creation)
  name: client_secret
  type: string
- description: Tenant the client belongs to
  name: tenant_id
  type: string
- description: Client type
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: Additional client metadata
  name: data
  type: object
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-client-schema.json
slug: account-management-client
source_filename: account-management-client-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-client-schema.json\",\n  \"title\": \"Client\",\n  \"description\": \"OAuth2 client credential\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth2 client identifier\",\n      \"example\": \"abc123def456\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth2 client secret (only shown on creation)\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Tenant the client belongs to\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"api_client\",\n        \"agent\"\n      ],\n      \"description\": \"Client type\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"enabled\",\n        \"disabled\"\n      ]\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional client metadata\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-client-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Client
---
