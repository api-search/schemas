---
description: Contains the password profile associated with a user. The passwordProfile property of the user entity is a passwordProfile object.
layout: schema
name: PasswordProfile
properties_list:
- description: The password for the user. Must satisfy the password complexity requirements of the tenant. Required on create.
  name: password
  type: string
- description: true if the user must change the password on the next sign-in; false otherwise
  name: forceChangePasswordNextSignIn
  type: boolean
- description: true if the user must perform multi-factor authentication before being forced to change the password
  name: forceChangePasswordNextSignInWithMfa
  type: boolean
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-password-profile-schema.json
slug: microsoft-entra-graph-identity-password-profile
source_filename: microsoft-entra-graph-identity-password-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PasswordProfile\",\n  \"type\": \"object\",\n  \"description\": \"Contains the password profile associated with a user. The passwordProfile property of the user entity is a passwordProfile object.\",\n  \"properties\": {\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for the user. Must satisfy the password complexity requirements of the tenant. Required on create.\"\n    },\n    \"forceChangePasswordNextSignIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if the user must change the password on the next sign-in; false otherwise\"\n    },\n    \"forceChangePasswordNextSignInWithMfa\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if the user must perform multi-factor authentication before being forced to change the password\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-password-profile-schema.json
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
title: PasswordProfile
---
