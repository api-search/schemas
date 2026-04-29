---
description: Specifies the set of OAuth 2.0 permission scopes and app roles under a specified resource that an application requires access to
layout: schema
name: RequiredResourceAccess
properties_list:
- description: The unique identifier for the resource that the application requires access to (the appId of the target application)
  name: resourceAppId
  type: string
- description: The list of OAuth 2.0 permission scopes and app roles required from the specified resource
  name: resourceAccess
  type: array
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-required-resource-access-schema.json
slug: microsoft-entra-graph-identity-required-resource-access
source_filename: microsoft-entra-graph-identity-required-resource-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequiredResourceAccess\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the set of OAuth 2.0 permission scopes and app roles under a specified resource that an application requires access to\",\n  \"properties\": {\n    \"resourceAppId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the resource that the application requires access to (the appId of the target application)\"\n    },\n    \"resourceAccess\": {\n      \"type\": \"array\",\n      \"description\": \"The list of OAuth 2.0 permission scopes and app roles required from the specified resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-required-resource-access-schema.json
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
title: RequiredResourceAccess
---
