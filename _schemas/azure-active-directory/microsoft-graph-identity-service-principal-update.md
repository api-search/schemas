---
description: Properties that can be updated on an existing service principal.
layout: schema
name: ServicePrincipalUpdate
properties_list:
- description: ''
  name: accountEnabled
  type: boolean
- description: ''
  name: appRoleAssignmentRequired
  type: boolean
- description: ''
  name: displayName
  type: string
- description: ''
  name: homepage
  type: string
- description: ''
  name: loginUrl
  type: string
- description: ''
  name: logoutUrl
  type: string
- description: ''
  name: notificationEmailAddresses
  type: array
- description: ''
  name: replyUrls
  type: array
- description: ''
  name: tags
  type: array
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-service-principal-update-schema.json
slug: microsoft-graph-identity-service-principal-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServicePrincipalUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Properties that can be updated on an existing service principal.\",\n  \"properties\": {\n    \"accountEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"appRoleAssignmentRequired\": {\n      \"type\": \"boolean\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"homepage\": {\n      \"type\": \"string\"\n    },\n    \"loginUrl\": {\n      \"type\": \"string\"\n    },\n    \"logoutUrl\": {\n      \"type\": \"string\"\n    },\n    \"notificationEmailAddresses\": {\n      \"type\": \"array\"\n    },\n    \"replyUrls\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-service-principal-update-schema.json
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
title: ServicePrincipalUpdate
---
