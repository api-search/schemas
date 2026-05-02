---
description: Properties required when creating a new service principal.
layout: schema
name: ServicePrincipalCreate
properties_list:
- description: The appId of the application to create a service principal for.
  name: appId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: accountEnabled
  type: boolean
- description: ''
  name: appRoleAssignmentRequired
  type: boolean
- description: ''
  name: tags
  type: array
- description: ''
  name: notificationEmailAddresses
  type: array
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-service-principal-create-schema.json
slug: microsoft-graph-identity-service-principal-create
source_filename: microsoft-graph-identity-service-principal-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServicePrincipalCreate\",\n  \"type\": \"object\",\n  \"description\": \"Properties required when creating a new service principal.\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The appId of the application to create a service principal for.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"accountEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"appRoleAssignmentRequired\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"notificationEmailAddresses\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-service-principal-create-schema.json
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
title: ServicePrincipalCreate
---
