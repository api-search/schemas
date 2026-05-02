---
description: Contains the password profile associated with a user.
layout: schema
name: PasswordProfile
properties_list:
- description: True if the user must change their password on the next sign-in.
  name: forceChangePasswordNextSignIn
  type: boolean
- description: If true, the user must perform multi-factor authentication before being forced to change their password.
  name: forceChangePasswordNextSignInWithMfa
  type: boolean
- description: The password for the user. Must satisfy the tenant's password complexity requirements. Setting a strong password is recommended.
  name: password
  type: string
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-password-profile-schema.json
slug: microsoft-graph-identity-password-profile
source_filename: microsoft-graph-identity-password-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PasswordProfile\",\n  \"type\": \"object\",\n  \"description\": \"Contains the password profile associated with a user.\",\n  \"properties\": {\n    \"forceChangePasswordNextSignIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the user must change their password on the next sign-in.\"\n    },\n    \"forceChangePasswordNextSignInWithMfa\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the user must perform multi-factor authentication before being forced to change their password.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for the user. Must satisfy the tenant's password complexity requirements. Setting a strong password is recommended.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-password-profile-schema.json
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
title: PasswordProfile
---
