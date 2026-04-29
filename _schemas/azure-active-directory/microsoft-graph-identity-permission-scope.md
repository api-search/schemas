---
description: Represents a delegated permission (OAuth2 scope).
layout: schema
name: PermissionScope
properties_list:
- description: ''
  name: adminConsentDescription
  type: string
- description: ''
  name: adminConsentDisplayName
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: isEnabled
  type: boolean
- description: ''
  name: type
  type: string
- description: ''
  name: userConsentDescription
  type: string
- description: ''
  name: userConsentDisplayName
  type: string
- description: The value to include in the scp claim in access tokens.
  name: value
  type: string
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-permission-scope-schema.json
slug: microsoft-graph-identity-permission-scope
source_filename: microsoft-graph-identity-permission-scope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionScope\",\n  \"type\": \"object\",\n  \"description\": \"Represents a delegated permission (OAuth2 scope).\",\n  \"properties\": {\n    \"adminConsentDescription\": {\n      \"type\": \"string\"\n    },\n    \"adminConsentDisplayName\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"userConsentDescription\": {\n      \"type\": \"string\"\n    },\n    \"userConsentDisplayName\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value to include in the scp claim in access tokens.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-permission-scope-schema.json
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
title: PermissionScope
---
