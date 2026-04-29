---
description: ''
layout: schema
name: CreateConnectionRequest
properties_list:
- description: Basiq institution ID for the bank
  name: institutionId
  type: string
- description: User's bank login ID
  name: loginId
  type: string
- description: User's bank password (encrypted in transit)
  name: password
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/createconnectionrequest.json
slug: createconnectionrequest
source_filename: createconnectionrequest.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/createconnectionrequest.json\",\n  \"title\": \"CreateConnectionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"institutionId\": {\n      \"type\": \"string\",\n      \"description\": \"Basiq institution ID for the bank\"\n    },\n    \"loginId\": {\n      \"type\": \"string\",\n      \"description\": \"User's bank login ID\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"User's bank password (encrypted in transit)\"\n    }\n  },\n  \"required\": [\n    \"institutionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/createconnectionrequest.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: CreateConnectionRequest
---
