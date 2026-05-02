---
description: Properties required when creating a new application registration.
layout: schema
name: ApplicationCreate
properties_list:
- description: The display name for the application.
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: signInAudience
  type: string
- description: ''
  name: identifierUris
  type: array
- description: ''
  name: appRoles
  type: array
- description: ''
  name: requiredResourceAccess
  type: array
- description: ''
  name: tags
  type: array
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-application-create-schema.json
slug: microsoft-graph-identity-application-create
source_filename: microsoft-graph-identity-application-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationCreate\",\n  \"type\": \"object\",\n  \"description\": \"Properties required when creating a new application registration.\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"signInAudience\": {\n      \"type\": \"string\"\n    },\n    \"identifierUris\": {\n      \"type\": \"array\"\n    },\n    \"appRoles\": {\n      \"type\": \"array\"\n    },\n    \"requiredResourceAccess\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-application-create-schema.json
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
title: ApplicationCreate
---
