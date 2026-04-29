---
description: ''
layout: schema
name: UserCreateRequest
properties_list:
- description: True if the account is enabled; otherwise, false.
  name: accountEnabled
  type: boolean
- description: The name to display in the address book for the user.
  name: displayName
  type: string
- description: The mail alias for the user.
  name: mailNickname
  type: string
- description: The user principal name (someuser@contoso.com).
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
  name: officeLocation
  type: string
- description: ''
  name: mobilePhone
  type: string
- description: ''
  name: usageLocation
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-user-create-request-schema.json
slug: microsoft-graph-user-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the account is enabled; otherwise, false.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name to display in the address book for the user.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the user.\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (someuser@contoso.com).\"\n    },\n    \"givenName\": {\n      \"type\": \"string\"\n    },\n    \"surname\": {\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    },\n    \"department\": {\n      \"type\": \"string\"\n    },\n    \"officeLocation\": {\n      \"type\": \"string\"\n  \
  \  },\n    \"mobilePhone\": {\n      \"type\": \"string\"\n    },\n    \"usageLocation\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-user-create-request-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: UserCreateRequest
---
