---
description: ''
layout: schema
name: SecurityGroup
properties_list:
- description: ''
  name: id
  type: string
- description: The Microsoft Entra security group ID
  name: groupId
  type: string
- description: The security group code
  name: code
  type: string
- description: The security group display name
  name: displayName
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-security-group-schema.json
slug: automation-security-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"The Microsoft Entra security group ID\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The security group code\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The security group display name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-security-group-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: SecurityGroup
---
