---
description: TokenRequest schema from AT&T API
layout: schema
name: TokenRequest
properties_list:
- description: The App Key from your AT&T developer account
  name: client_id
  type: string
- description: The App Secret from your AT&T developer account
  name: client_secret
  type: string
- description: OAuth grant type
  name: grant_type
  type: string
- description: Space-separated list of API scopes (e.g. SMS, MMS, SPEECH)
  name: scope
  type: string
- description: Authorization code (required for authorization_code grant type)
  name: code
  type: string
- description: Refresh token (required for refresh_token grant type)
  name: refresh_token
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-token-request-schema.json
slug: sms-api-token-request
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: TokenRequest
---
