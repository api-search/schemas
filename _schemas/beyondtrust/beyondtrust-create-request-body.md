---
description: Request body for creating an access request.
layout: schema
name: CreateRequestBody
properties_list:
- description: ID of the managed system.
  name: SystemID
  type: integer
- description: ID of the managed account.
  name: AccountID
  type: integer
- description: Requested access duration in minutes.
  name: DurationMinutes
  type: integer
- description: Business justification for the access request.
  name: Reason
  type: string
- description: Type of access requested.
  name: AccessType
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-create-request-body-schema.json
slug: beyondtrust-create-request-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-create-request-body-schema.json\",\n  \"title\": \"CreateRequestBody\",\n  \"description\": \"Request body for creating an access request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SystemID\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the managed system.\",\n      \"example\": 10\n    },\n    \"AccountID\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the managed account.\",\n      \"example\": 20\n    },\n    \"DurationMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Requested access duration in minutes.\",\n      \"example\": 60\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"description\": \"Business justification for the access request.\",\n      \"example\": \"Maintenance window access\"\n    },\n \
  \   \"AccessType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of access requested.\",\n      \"enum\": [\n        \"View\",\n        \"RDP\",\n        \"SSH\",\n        \"App\"\n      ],\n      \"example\": \"View\"\n    }\n  },\n  \"required\": [\n    \"SystemID\",\n    \"AccountID\",\n    \"DurationMinutes\",\n    \"Reason\",\n    \"AccessType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-create-request-body-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: CreateRequestBody
---
