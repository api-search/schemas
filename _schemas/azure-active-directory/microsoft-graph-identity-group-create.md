---
description: Properties required when creating a new group.
layout: schema
name: GroupCreate
properties_list:
- description: The display name for the group.
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: Set to ["Unified"] for Microsoft 365 groups. Omit for security groups.
  name: groupTypes
  type: array
- description: ''
  name: mailEnabled
  type: boolean
- description: ''
  name: mailNickname
  type: string
- description: ''
  name: securityEnabled
  type: boolean
- description: ''
  name: visibility
  type: string
- description: ''
  name: isAssignableToRole
  type: boolean
- description: 'List of directory object URLs to add as members. Example: https://graph.microsoft.com/v1.0/directoryObjects/{id}'
  name: members@odata.bind
  type: array
- description: List of directory object URLs to set as owners.
  name: owners@odata.bind
  type: array
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-group-create-schema.json
slug: microsoft-graph-identity-group-create
source_filename: microsoft-graph-identity-group-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupCreate\",\n  \"type\": \"object\",\n  \"description\": \"Properties required when creating a new group.\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the group.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"groupTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Set to [\\\"Unified\\\"] for Microsoft 365 groups. Omit for security groups.\"\n    },\n    \"mailEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\"\n    },\n    \"securityEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"visibility\": {\n      \"type\": \"string\"\n    },\n    \"isAssignableToRole\": {\n      \"type\": \"boolean\"\n    },\n    \"members@odata.bind\": {\n      \"type\": \"array\",\n      \"description\": \"List of directory object URLs\
  \ to add as members. Example: https://graph.microsoft.com/v1.0/directoryObjects/{id}\"\n    },\n    \"owners@odata.bind\": {\n      \"type\": \"array\",\n      \"description\": \"List of directory object URLs to set as owners.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-group-create-schema.json
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
title: GroupCreate
---
