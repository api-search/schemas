---
description: CreatePlayerSessionInput schema from Amazon GameLift API
layout: schema
name: CreatePlayerSessionInput
properties_list:
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: PlayerData
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-player-session-input-schema.json
slug: gamelift-create-player-session-input
source_filename: gamelift-create-player-session-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-session-input-schema.json\",\n  \"title\": \"CreatePlayerSessionInput\",\n  \"description\": \"CreatePlayerSessionInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session to add a player to.\"\n        }\n      ]\n    },\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player. Player IDs are developer-defined.\"\n        }\n      ]\n    },\n    \"PlayerData\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/PlayerData\"\n        },\n        {\n          \"description\": \"Developer-defined information related to a player. Amazon GameLift does not use this data, so it can be formatted as needed for use in the game.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameSessionId\",\n    \"PlayerId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-session-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreatePlayerSessionInput
---
