---
description: Password profile for a Microsoft Entra user account
layout: schema
name: PasswordProfile
properties_list:
- description: Password for the user — must meet tenant complexity requirements
  name: password
  type: string
- description: If true, user must reset password at next sign-in
  name: forceChangePasswordNextSignIn
  type: boolean
- description: If true, user must perform MFA and then reset password at next sign-in
  name: forceChangePasswordNextSignInWithMfa
  type: boolean
provider_name: Microsoft Active Directory
provider_slug: active-directory
schema_file: json-schema/users-password-profile-schema.json
slug: users-password-profile
source_filename: users-password-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/active-directory/main/json-schema/users-password-profile-schema.json\",\n  \"title\": \"PasswordProfile\",\n  \"description\": \"Password profile for a Microsoft Entra user account\",\n  \"type\": \"object\",\n  \"required\": [\"password\"],\n  \"properties\": {\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for the user — must meet tenant complexity requirements\",\n      \"writeOnly\": true,\n      \"minLength\": 8\n    },\n    \"forceChangePasswordNextSignIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, user must reset password at next sign-in\",\n      \"default\": true\n    },\n    \"forceChangePasswordNextSignInWithMfa\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, user must perform MFA and then reset password at next sign-in\",\n      \"default\": false\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/json-schema/users-password-profile-schema.json
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
title: PasswordProfile
---
