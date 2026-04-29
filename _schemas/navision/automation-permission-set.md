---
description: ''
layout: schema
name: PermissionSet
properties_list:
- description: ''
  name: id
  type: string
- description: The permission set role ID
  name: roleId
  type: string
- description: The permission set display name
  name: displayName
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: appId
  type: string
- description: ''
  name: extensionName
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-permission-set-schema.json
slug: automation-permission-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionSet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"roleId\": {\n      \"type\": \"string\",\n      \"description\": \"The permission set role ID\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The permission set display name\"\n    },\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"extensionName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-permission-set-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: PermissionSet
---
