---
description: Request body for retrieving player information.
layout: schema
name: PlayerInfoRequest
properties_list:
- description: The merchant's unique identifier.
  name: merchantId
  type: string
- description: The player's unique identifier.
  name: playerId
  type: string
- description: SHA-256 hash for request authentication.
  name: hash
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-player-info-request-schema.json
slug: wallet-api-player-info-request
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: PlayerInfoRequest
---
