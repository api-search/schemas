---
description: Authenticated user session details.
layout: schema
name: SessionResponse
properties_list:
- description: Internal user ID.
  name: UserId
  type: integer
- description: Email address of the authenticated user.
  name: EmailAddress
  type: string
- description: Username of the authenticated user.
  name: UserName
  type: string
- description: Display name of the authenticated user.
  name: Name
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-session-response-schema.json
slug: beyondtrust-session-response
source_filename: beyondtrust-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-session-response-schema.json\",\n  \"title\": \"SessionResponse\",\n  \"description\": \"Authenticated user session details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserId\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal user ID.\",\n      \"example\": 42\n    },\n    \"EmailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the authenticated user.\",\n      \"example\": \"apiuser@example.com\"\n    },\n    \"UserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the authenticated user.\",\n      \"example\": \"api-service-account\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the authenticated user.\",\n      \"example\"\
  : \"API Service Account\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-session-response-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: SessionResponse
---
