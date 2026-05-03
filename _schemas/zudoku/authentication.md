---
description: Schema for the Zudoku authentication configuration that enables user sign-in, API key management, and identity-based API playground access through OpenID Connect, OAuth2, or custom providers.
layout: schema
name: Zudoku Authentication Configuration
properties_list:
- description: The authentication provider type.
  name: type
  type: string
- description: OAuth2 or OpenID Connect client identifier.
  name: clientId
  type: string
- description: OpenID Connect issuer URL for token verification and discovery.
  name: issuer
  type: string
- description: Requested OAuth2 scopes for the authentication flow.
  name: scopes
  type: array
- description: OAuth2 redirect URI after successful authentication.
  name: redirectUri
  type: string
- description: OAuth2 audience parameter for token requests.
  name: audience
  type: string
provider_name: Zudoku
provider_slug: zudoku
schema_file: json-schema/authentication.json
slug: authentication
source_filename: authentication.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zudoku/blob/main/json-schema/authentication.json\",\n  \"title\": \"Zudoku Authentication Configuration\",\n  \"description\": \"Schema for the Zudoku authentication configuration that enables user sign-in, API key management, and identity-based API playground access through OpenID Connect, OAuth2, or custom providers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"openid\", \"oauth2\", \"custom\"],\n      \"description\": \"The authentication provider type.\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth2 or OpenID Connect client identifier.\"\n    },\n    \"issuer\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"OpenID Connect issuer URL for token verification and discovery.\"\n    },\n    \"scopes\": {\n    \
  \  \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Requested OAuth2 scopes for the authentication flow.\"\n    },\n    \"redirectUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"OAuth2 redirect URI after successful authentication.\"\n    },\n    \"audience\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth2 audience parameter for token requests.\"\n    }\n  },\n  \"required\": [\"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/json-schema/authentication.json
tags:
- Developer Tools
- Documentation
title: Zudoku Authentication Configuration
---
