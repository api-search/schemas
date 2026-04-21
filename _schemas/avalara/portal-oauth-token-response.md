---
description: TokenResponse schema from Avalara API
layout: schema
name: TokenResponse
properties_list:
- description: The OAuth 2.0 access token
  name: access_token
  type: string
- description: ''
  name: token_type
  type: string
- description: Token expiry time in seconds
  name: expires_in
  type: integer
- description: Granted scopes
  name: scope
  type: string
- description: Refresh token (if applicable)
  name: refresh_token
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/portal-oauth-token-response-schema.json
slug: portal-oauth-token-response
tags:
- Taxes
title: TokenResponse
---
