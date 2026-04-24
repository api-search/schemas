---
description: A paginated list of Hearthstone card backs.
layout: schema
name: CardBackSearchResponse
properties_list:
- description: List of matching card backs.
  name: cardBacks
  type: array
- description: Total number of matching card backs.
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
schema_file: json-schema/hearthstone-game-data-card-back-search-response-schema.json
slug: hearthstone-game-data-card-back-search-response
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: CardBackSearchResponse
---
