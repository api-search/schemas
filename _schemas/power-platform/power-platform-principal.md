---
description: Represents a principal (user or service principal) that performed an action.
layout: schema
name: Principal
properties_list:
- description: The unique identifier of the principal.
  name: id
  type: string
- description: The display name of the principal.
  name: displayName
  type: '[''string'', ''null'']'
- description: The type of principal.
  name: type
  type: string
- description: The tenant ID of the principal.
  name: tenantId
  type: '[''string'', ''null'']'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-principal-schema.json
slug: power-platform-principal
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Principal\",\n  \"type\": \"object\",\n  \"description\": \"Represents a principal (user or service principal) that performed an action.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the principal.\"\n    },\n    \"displayName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The display name of the principal.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of principal.\"\n    },\n    \"tenantId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The tenant ID of the principal.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-principal-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: Principal
---
