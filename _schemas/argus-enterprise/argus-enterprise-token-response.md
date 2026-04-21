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
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: TokenResponse
---
