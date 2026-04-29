---
description: Player information for use when creating player sessions using a game session placement request.
layout: schema
name: DesiredPlayerSession
properties_list:
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: PlayerData
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-desired-player-session-schema.json
slug: gamelift-desired-player-session
source_filename: gamelift-desired-player-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-desired-player-session-schema.json\",\n  \"title\": \"DesiredPlayerSession\",\n  \"description\": \"Player information for use when creating player sessions using a game session placement request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player to associate with the player session.\"\n        }\n      ]\n    },\n    \"PlayerData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerData\"\n        },\n        {\n          \"description\": \"Developer-defined information related to a player. Amazon GameLift does not use this data, so it can be formatted as needed\
  \ for use in the game.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-desired-player-session-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DesiredPlayerSession
---
