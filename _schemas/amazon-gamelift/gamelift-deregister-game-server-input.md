---
description: DeregisterGameServerInput schema from Amazon GameLift API
layout: schema
name: DeregisterGameServerInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: GameServerId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-deregister-game-server-input-schema.json
slug: gamelift-deregister-game-server-input
source_filename: gamelift-deregister-game-server-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-deregister-game-server-input-schema.json\",\n  \"title\": \"DeregisterGameServerInput\",\n  \"description\": \"DeregisterGameServerInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group where the game server is running.\"\n        }\n      ]\n    },\n    \"GameServerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerId\"\n        },\n        {\n          \"description\": \"A custom string that uniquely identifies the game server to deregister.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"GameServerGroupName\",\n    \"GameServerId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-deregister-game-server-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeregisterGameServerInput
---
