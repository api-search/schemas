---
description: OData reference link used to add relationships
layout: schema
name: ODataReference
properties_list:
- description: 'The full URL to the directory object to add as a member. Format: https://graph.microsoft.com/v1.0/directoryObjects/{id}'
  name: '@odata.id'
  type: string
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-o-data-reference-schema.json
slug: microsoft-entra-graph-identity-o-data-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ODataReference\",\n  \"type\": \"object\",\n  \"description\": \"OData reference link used to add relationships\",\n  \"properties\": {\n    \"@odata.id\": {\n      \"type\": \"string\",\n      \"description\": \"The full URL to the directory object to add as a member. Format: https://graph.microsoft.com/v1.0/directoryObjects/{id}\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-o-data-reference-schema.json
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
title: ODataReference
---
