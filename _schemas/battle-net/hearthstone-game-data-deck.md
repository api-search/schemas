---
description: A Hearthstone deck.
layout: schema
name: Deck
properties_list:
- description: The deck code string.
  name: deckCode
  type: string
- description: The deck version.
  name: version
  type: integer
- description: The deck format (standard, wild, classic).
  name: format
  type: string
- description: The class associated with a deck.
  name: class
  type: object
- description: The cards in the deck.
  name: cards
  type: array
- description: Total number of cards in the deck.
  name: cardCount
  type: integer
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-deck-schema.json
slug: hearthstone-game-data-deck
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: Deck
---
