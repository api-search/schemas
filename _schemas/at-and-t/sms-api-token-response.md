---
description: TokenResponse schema from AT&T API
layout: schema
name: TokenResponse
properties_list:
- description: OAuth access token valid for 2 days (172800 seconds)
  name: access_token
  type: string
- description: Token expiration time in seconds (default 172800)
  name: expires_in
  type: integer
- description: Refresh token valid for 90 days
  name: refresh_token
  type: string
- description: Token type (always BEARER)
  name: token_type
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-token-response-schema.json
slug: sms-api-token-response
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: TokenResponse
---
