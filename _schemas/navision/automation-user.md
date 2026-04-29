---
description: ''
layout: schema
name: User
properties_list:
- description: The user security ID
  name: userSecurityId
  type: string
- description: The user name
  name: userName
  type: string
- description: The user display name
  name: displayName
  type: string
- description: The user state
  name: state
  type: string
- description: The user expiry date
  name: expiryDate
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-user-schema.json
slug: automation-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userSecurityId\": {\n      \"type\": \"string\",\n      \"description\": \"The user security ID\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The user name\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The user display name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The user state\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"The user expiry date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-user-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: User
---
