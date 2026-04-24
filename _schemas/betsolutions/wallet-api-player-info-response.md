---
description: Player profile and account information.
layout: schema
name: PlayerInfoResponse
properties_list:
- description: Whether the request succeeded.
  name: success
  type: boolean
- description: Unique player user ID.
  name: userId
  type: string
- description: Player's username.
  name: userName
  type: string
- description: Player's first name.
  name: firstName
  type: string
- description: Player's last name.
  name: lastName
  type: string
- description: Player's email address.
  name: email
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: countryCode
  type: string
- description: ISO 4217 currency code for the player's account.
  name: currency
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-player-info-response-schema.json
slug: wallet-api-player-info-response
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: PlayerInfoResponse
---
