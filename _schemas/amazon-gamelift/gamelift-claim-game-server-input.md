---
description: ClaimGameServerInput schema from Amazon GameLift API
layout: schema
name: ClaimGameServerInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: GameServerId
  type: object
- description: ''
  name: GameServerData
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-claim-game-server-input-schema.json
slug: gamelift-claim-game-server-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-claim-game-server-input-schema.json\",\n  \"title\": \"ClaimGameServerInput\",\n  \"description\": \"ClaimGameServerInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group where the game server is running. If you are not specifying a game server to claim, this value identifies where you want Amazon GameLift FleetIQ to look for an available game server to claim. \"\n        }\n      ]\n    },\n    \"GameServerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerId\"\n        },\n        {\n     \
  \     \"description\": \"A custom string that uniquely identifies the game server to claim. If this parameter is left empty, Amazon GameLift FleetIQ searches for an available game server in the specified game server group.\"\n        }\n      ]\n    },\n    \"GameServerData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerData\"\n        },\n        {\n          \"description\": \"A set of custom game server properties, formatted as a single string value. This data is passed to a game client or service when it requests information on game servers. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-claim-game-server-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ClaimGameServerInput
---
