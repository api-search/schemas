---
description: Authentication response with private player token.
layout: schema
name: AuthResponse
properties_list:
- description: Whether authentication succeeded.
  name: success
  type: boolean
- description: Private player token for subsequent API calls.
  name: token
  type: string
- description: Unique player identifier.
  name: playerId
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-auth-response-schema.json
slug: wallet-api-auth-response
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: AuthResponse
---
