---
description: A paginated list of Hearthstone cards.
layout: schema
name: CardSearchResponse
properties_list:
- description: List of matching cards.
  name: cards
  type: array
- description: Total number of matching cards.
  name: cardCount
  type: integer
- description: Total number of pages.
  name: pageCount
  type: integer
- description: Current page number.
  name: page
  type: integer
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-card-search-response-schema.json
slug: hearthstone-game-data-card-search-response
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: CardSearchResponse
---
