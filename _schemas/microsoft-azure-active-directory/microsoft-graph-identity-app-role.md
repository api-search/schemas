---
description: Represents an application role that can be assigned to users, groups, or service principals.
layout: schema
name: AppRole
properties_list:
- description: Specifies whether this app role can be assigned to users and groups or to applications.
  name: allowedMemberTypes
  type: array
- description: ''
  name: description
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: isEnabled
  type: boolean
- description: The value to include in the roles claim in access tokens.
  name: value
  type: string
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-app-role-schema.json
slug: microsoft-graph-identity-app-role
source_filename: microsoft-graph-identity-app-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppRole\",\n  \"type\": \"object\",\n  \"description\": \"Represents an application role that can be assigned to users, groups, or service principals.\",\n  \"properties\": {\n    \"allowedMemberTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies whether this app role can be assigned to users and groups or to applications.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value to include in the roles claim in access tokens.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-app-role-schema.json
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
title: AppRole
---
