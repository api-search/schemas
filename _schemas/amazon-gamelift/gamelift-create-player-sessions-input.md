---
description: CreatePlayerSessionsInput schema from Amazon GameLift API
layout: schema
name: CreatePlayerSessionsInput
properties_list:
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: PlayerIds
  type: object
- description: ''
  name: PlayerDataMap
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-player-sessions-input-schema.json
slug: gamelift-create-player-sessions-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-sessions-input-schema.json\",\n  \"title\": \"CreatePlayerSessionsInput\",\n  \"description\": \"CreatePlayerSessionsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session to add players to.\"\n        }\n      ]\n    },\n    \"PlayerIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerIdList\"\n        },\n        {\n          \"description\": \"List of unique identifiers for the players to be added.\"\n        }\n      ]\n    },\n    \"PlayerDataMap\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PlayerDataMap\"\n        },\n        {\n          \"description\": \"Map of string pairs, each specifying a player ID and a set of developer-defined information related to the player. Amazon GameLift does not use this data, so it can be formatted as needed for use in the game. Any player data strings for player IDs that are not included in the <code>PlayerIds</code> parameter are ignored. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameSessionId\",\n    \"PlayerIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-sessions-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreatePlayerSessionsInput
---
