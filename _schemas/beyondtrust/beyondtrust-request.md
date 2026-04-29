---
description: An access request for a privileged account.
layout: schema
name: Request
properties_list:
- description: Unique identifier of the request.
  name: RequestID
  type: integer
- description: Current status of the request.
  name: Status
  type: string
- description: Type of access requested.
  name: AccessType
  type: string
- description: Name of the privileged account.
  name: AccountName
  type: string
- description: ID of the managed account.
  name: AccountID
  type: integer
- description: Name of the target system.
  name: SystemName
  type: string
- description: ID of the managed system.
  name: SystemID
  type: integer
- description: When the approved request expires.
  name: ExpiresDate
  type: string
- description: Requested duration in minutes.
  name: RequestedDurationMinutes
  type: integer
- description: Reason provided for the access request.
  name: Reason
  type: string
- description: When the request was created.
  name: RequestDate
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-request-schema.json
slug: beyondtrust-request
source_filename: beyondtrust-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-request-schema.json\",\n  \"title\": \"Request\",\n  \"description\": \"An access request for a privileged account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the request.\",\n      \"example\": 1001\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the request.\",\n      \"enum\": [\n        \"Pending\",\n        \"Approved\",\n        \"Denied\",\n        \"Expired\",\n        \"Cancelled\"\n      ],\n      \"example\": \"Approved\"\n    },\n    \"AccessType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of access requested.\",\n      \"enum\": [\n        \"View\",\n        \"RDP\",\n        \"SSH\",\n        \"App\"\n   \
  \   ],\n      \"example\": \"View\"\n    },\n    \"AccountName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the privileged account.\",\n      \"example\": \"administrator\"\n    },\n    \"AccountID\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the managed account.\",\n      \"example\": 20\n    },\n    \"SystemName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target system.\",\n      \"example\": \"prod-server-01\"\n    },\n    \"SystemID\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the managed system.\",\n      \"example\": 10\n    },\n    \"ExpiresDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the approved request expires.\",\n      \"example\": \"2026-04-19T12:00:00Z\"\n    },\n    \"RequestedDurationMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Requested duration in minutes.\",\n     \
  \ \"example\": 60\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Reason provided for the access request.\",\n      \"example\": \"Maintenance window access\"\n    },\n    \"RequestDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the request was created.\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-request-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: Request
---
