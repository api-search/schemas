---
description: Properties that can be updated on an existing application.
layout: schema
name: ApplicationUpdate
properties_list:
- description: ''
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
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-application-update-schema.json
slug: microsoft-graph-identity-application-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Properties that can be updated on an existing application.\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"signInAudience\": {\n      \"type\": \"string\"\n    },\n    \"identifierUris\": {\n      \"type\": \"array\"\n    },\n    \"appRoles\": {\n      \"type\": \"array\"\n    },\n    \"requiredResourceAccess\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-application-update-schema.json
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
title: ApplicationUpdate
---
