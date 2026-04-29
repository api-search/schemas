---
description: Contains the password profile associated with a user.
layout: schema
name: PasswordProfile
properties_list:
- description: Whether the user must change the password on the next sign-in.
  name: forceChangePasswordNextSignIn
  type: boolean
- description: Whether the user must perform multi-factor authentication before being forced to change their password.
  name: forceChangePasswordNextSignInWithMfa
  type: boolean
- description: The password for the user. Must satisfy the tenant's password complexity requirements. Minimum of 8 characters.
  name: password
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-password-profile-schema.json
slug: microsoft-graph-password-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PasswordProfile\",\n  \"type\": \"object\",\n  \"description\": \"Contains the password profile associated with a user.\",\n  \"properties\": {\n    \"forceChangePasswordNextSignIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user must change the password on the next sign-in.\"\n    },\n    \"forceChangePasswordNextSignInWithMfa\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user must perform multi-factor authentication before being forced to change their password.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for the user. Must satisfy the tenant's password complexity requirements. Minimum of 8 characters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-password-profile-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: PasswordProfile
---
