---
description: Specifies the set of OAuth 2.0 permission scopes and app roles that an application requires access to.
layout: schema
name: RequiredResourceAccess
properties_list:
- description: The unique identifier for the resource that the application requires access to (e.g., Microsoft Graph).
  name: resourceAppId
  type: string
- description: ''
  name: resourceAccess
  type: array
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-required-resource-access-schema.json
slug: microsoft-graph-identity-required-resource-access
source_filename: microsoft-graph-identity-required-resource-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequiredResourceAccess\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the set of OAuth 2.0 permission scopes and app roles that an application requires access to.\",\n  \"properties\": {\n    \"resourceAppId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the resource that the application requires access to (e.g., Microsoft Graph).\"\n    },\n    \"resourceAccess\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-required-resource-access-schema.json
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
title: RequiredResourceAccess
---
