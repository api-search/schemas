---
description: A privileged account managed by BeyondTrust Password Safe.
layout: schema
name: ManagedAccount
properties_list:
- description: Unique identifier of the managed account.
  name: AccountID
  type: integer
- description: Name of the privileged account.
  name: AccountName
  type: string
- description: ID of the managed system.
  name: SystemID
  type: integer
- description: Name of the system containing this account.
  name: SystemName
  type: string
- description: Domain name for domain accounts.
  name: DomainName
  type: string
- description: Type of account.
  name: AccountType
  type: string
- description: When the password was last changed.
  name: LastChangeDate
  type: string
- description: Whether password fallback is enabled.
  name: PasswordFallbackFlag
  type: boolean
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-managed-account-schema.json
slug: beyondtrust-managed-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-managed-account-schema.json\",\n  \"title\": \"ManagedAccount\",\n  \"description\": \"A privileged account managed by BeyondTrust Password Safe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the managed account.\",\n      \"example\": 20\n    },\n    \"AccountName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the privileged account.\",\n      \"example\": \"administrator\"\n    },\n    \"SystemID\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the managed system.\",\n      \"example\": 10\n    },\n    \"SystemName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the system containing this account.\",\n      \"example\": \"prod-server-01\"\
  \n    },\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Domain name for domain accounts.\",\n      \"example\": \"example.com\"\n    },\n    \"AccountType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of account.\",\n      \"enum\": [\n        \"Local\",\n        \"Domain\",\n        \"ServiceAccount\"\n      ],\n      \"example\": \"Local\"\n    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the password was last changed.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    },\n    \"PasswordFallbackFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether password fallback is enabled.\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-managed-account-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: ManagedAccount
---
