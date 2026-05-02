---
description: Properties required when creating a new user.
layout: schema
name: UserCreate
properties_list:
- description: True if the account should be enabled.
  name: accountEnabled
  type: boolean
- description: The name to display in the address book.
  name: displayName
  type: string
- description: The mail alias for the user.
  name: mailNickname
  type: string
- description: The user principal name (user@contoso.com).
  name: userPrincipalName
  type: string
- description: ''
  name: givenName
  type: string
- description: ''
  name: surname
  type: string
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: department
  type: string
- description: ''
  name: usageLocation
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: mobilePhone
  type: string
- description: ''
  name: businessPhones
  type: array
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-user-create-schema.json
slug: microsoft-graph-identity-user-create
source_filename: microsoft-graph-identity-user-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCreate\",\n  \"type\": \"object\",\n  \"description\": \"Properties required when creating a new user.\",\n  \"properties\": {\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the account should be enabled.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name to display in the address book.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the user.\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (user@contoso.com).\"\n    },\n    \"givenName\": {\n      \"type\": \"string\"\n    },\n    \"surname\": {\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    },\n    \"department\": {\n      \"type\": \"string\"\n    },\n    \"usageLocation\"\
  : {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\"\n    },\n    \"businessPhones\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-user-create-schema.json
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
title: UserCreate
---
