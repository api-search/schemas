---
description: Contains a password credential (client secret) associated with an application or service principal.
layout: schema
name: PasswordCredential
properties_list:
- description: ''
  name: customKeyIdentifier
  type: '[''string'', ''null'']'
- description: ''
  name: displayName
  type: '[''string'', ''null'']'
- description: The date and time at which the password expires.
  name: endDateTime
  type: string
- description: Contains the first three characters of the password.
  name: hint
  type: '[''string'', ''null'']'
- description: ''
  name: keyId
  type: string
- description: The client secret value. Only returned on creation; not retrievable afterward.
  name: secretText
  type: '[''string'', ''null'']'
- description: ''
  name: startDateTime
  type: string
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-password-credential-schema.json
slug: microsoft-graph-identity-password-credential
source_filename: microsoft-graph-identity-password-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PasswordCredential\",\n  \"type\": \"object\",\n  \"description\": \"Contains a password credential (client secret) associated with an application or service principal.\",\n  \"properties\": {\n    \"customKeyIdentifier\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"displayName\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time at which the password expires.\"\n    },\n    \"hint\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Contains the first three characters of the password.\"\n    },\n    \"keyId\": {\n      \"type\": \"string\"\n    },\n    \"secretText\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The client secret value. Only returned on creation; not retrievable afterward.\"\n    },\n    \"startDateTime\": {\n      \"type\"\
  : \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-password-credential-schema.json
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
title: PasswordCredential
---
