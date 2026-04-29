---
description: Represents a password credential (client secret) associated with an application or service principal
layout: schema
name: PasswordCredential
properties_list:
- description: Unique identifier for the password
  name: keyId
  type: string
- description: Friendly name for the password credential
  name: displayName
  type: '[''string'', ''null'']'
- description: Contains the first three characters of the password (returned on read operations)
  name: hint
  type: string
- description: The generated password value. Only returned at creation time and cannot be retrieved later.
  name: secretText
  type: string
- description: The date and time at which the password becomes valid
  name: startDateTime
  type: string
- description: The date and time at which the password expires. Maximum lifetime varies by policy.
  name: endDateTime
  type: string
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-password-credential-schema.json
slug: microsoft-entra-graph-identity-password-credential
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PasswordCredential\",\n  \"type\": \"object\",\n  \"description\": \"Represents a password credential (client secret) associated with an application or service principal\",\n  \"properties\": {\n    \"keyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the password\"\n    },\n    \"displayName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Friendly name for the password credential\"\n    },\n    \"hint\": {\n      \"type\": \"string\",\n      \"description\": \"Contains the first three characters of the password (returned on read operations)\"\n    },\n    \"secretText\": {\n      \"type\": \"string\",\n      \"description\": \"The generated password value. Only returned at creation time and cannot be retrieved later.\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time at which\
  \ the password becomes valid\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time at which the password expires. Maximum lifetime varies by policy.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-password-credential-schema.json
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
title: PasswordCredential
---
