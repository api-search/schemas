---
description: A BetSolutions game with product metadata.
layout: schema
name: Game
properties_list:
- description: Unique game identifier.
  name: gameId
  type: string
- description: Product category ID (1=Table Games, 2=Slots, 3=Provably Fair).
  name: productId
  type: integer
- description: Game display name.
  name: name
  type: string
- description: Whether the game supports freespin/freeplay campaigns.
  name: hasFreePay
  type: boolean
- description: URL to launch the game.
  name: launchUrl
  type: string
- description: Return-to-player percentage.
  name: rtp
  type: number
- description: Rake percentage for the game.
  name: rakePercent
  type: number
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-game-schema.json
slug: wallet-api-game
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: Game
---
