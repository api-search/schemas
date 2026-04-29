---
description: Base type for many directory resources including users, groups, and service principals
layout: schema
name: DirectoryObject
properties_list:
- description: The OData type string for the directory object
  name: '@odata.type'
  type: string
- description: Unique identifier for the directory object
  name: id
  type: string
- description: The display name of the directory object
  name: displayName
  type: '[''string'', ''null'']'
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-directory-object-schema.json
slug: microsoft-entra-graph-identity-directory-object
source_filename: microsoft-entra-graph-identity-directory-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DirectoryObject\",\n  \"type\": \"object\",\n  \"description\": \"Base type for many directory resources including users, groups, and service principals\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"description\": \"The OData type string for the directory object\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the directory object\"\n    },\n    \"displayName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The display name of the directory object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-directory-object-schema.json
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
title: DirectoryObject
---
