---
description: TokenResponse schema from ARGUS Enterprise API
layout: schema
name: TokenResponse
properties_list:
- description: Bearer token for API authentication
  name: access_token
  type: string
- description: ''
  name: token_type
  type: string
- description: Token validity duration in seconds
  name: expires_in
  type: integer
- description: Granted scopes
  name: scope
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-token-response-schema.json
slug: argus-enterprise-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"TokenResponse schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"Bearer token for API authentication\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Bearer\"\n      ]\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token validity duration in seconds\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Granted scopes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-token-response-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: TokenResponse
---
