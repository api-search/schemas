---
description: A set of permissions that can be assigned to a role
layout: schema
name: PermissionSet
properties_list:
- description: Unique numeric identifier
  name: id
  type: integer
- description: Display name
  name: name
  type: string
- description: List of permission strings
  name: permissions
  type: array
- description: Whether this is a built-in permission set
  name: built_in
  type: boolean
- description: Whether this grants all permissions
  name: all_access
  type: boolean
- description: Relative URL
  name: url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-permission-set-schema.json
slug: looker-permission-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionSet\",\n  \"type\": \"object\",\n  \"description\": \"A set of permissions that can be assigned to a role\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"List of permission strings\"\n    },\n    \"built_in\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a built-in permission set\"\n    },\n    \"all_access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this grants all permissions\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-permission-set-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: PermissionSet
---
