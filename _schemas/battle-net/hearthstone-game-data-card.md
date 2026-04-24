---
description: A Hearthstone card object.
layout: schema
name: Card
properties_list:
- description: The card's unique ID.
  name: id
  type: integer
- description: Indicates if the card is collectible (1) or uncollectible (0).
  name: collectible
  type: integer
- description: A human-readable identifier for the card.
  name: slug
  type: string
- description: The class ID of the card.
  name: classId
  type: integer
- description: Class IDs if the card belongs to multiple classes.
  name: multiClassIds
  type: array
- description: The card type ID.
  name: cardTypeId
  type: integer
- description: The set ID of the card.
  name: cardSetId
  type: integer
- description: The rarity ID of the card.
  name: rarityId
  type: integer
- description: The name of the card's artist.
  name: artistName
  type: string
- description: The health of the minion.
  name: health
  type: integer
- description: The attack power of the card.
  name: attack
  type: integer
- description: The mana cost to play the card.
  name: manaCost
  type: integer
- description: The name of the card.
  name: name
  type: string
- description: The card's text.
  name: text
  type: string
- description: URL of the card image.
  name: image
  type: string
- description: Flavor text for the card.
  name: flavorText
  type: string
- description: URL of the cropped card image.
  name: cropImage
  type: string
- description: IDs of child cards.
  name: childIds
  type: array
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-card-schema.json
slug: hearthstone-game-data-card
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: Card
---
