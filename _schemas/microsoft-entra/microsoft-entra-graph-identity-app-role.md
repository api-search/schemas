---
description: Represents a role defined by an application that can be assigned to users, groups, or service principals
layout: schema
name: AppRole
properties_list:
- description: Unique identifier for the app role
  name: id
  type: string
- description: Specifies whether the role can be assigned to users/groups, applications, or both
  name: allowedMemberTypes
  type: array
- description: Display name for the app role
  name: displayName
  type: string
- description: Description of the app role
  name: description
  type: '[''string'', ''null'']'
- description: Value that is included in the roles claim in authentication tokens
  name: value
  type: '[''string'', ''null'']'
- description: Whether the app role is enabled
  name: isEnabled
  type: boolean
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-app-role-schema.json
slug: microsoft-entra-graph-identity-app-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppRole\",\n  \"type\": \"object\",\n  \"description\": \"Represents a role defined by an application that can be assigned to users, groups, or service principals\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the app role\"\n    },\n    \"allowedMemberTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies whether the role can be assigned to users/groups, applications, or both\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the app role\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Description of the app role\"\n    },\n    \"value\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Value that is included in the roles claim in authentication tokens\"\n    },\n    \"isEnabled\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the app role is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-app-role-schema.json
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
title: AppRole
---
