---
description: UpdateGameServerInput schema from Amazon GameLift API
layout: schema
name: UpdateGameServerInput
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
- description: ''
  name: UtilizationStatus
  type: object
- description: ''
  name: HealthCheck
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-game-server-input-schema.json
slug: gamelift-update-game-server-input
source_filename: gamelift-update-game-server-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-server-input-schema.json\",\n  \"title\": \"UpdateGameServerInput\",\n  \"description\": \"UpdateGameServerInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group where the game server is running.\"\n        }\n      ]\n    },\n    \"GameServerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerId\"\n        },\n        {\n          \"description\": \"A custom string that uniquely identifies the game server to update.\"\n        }\n      ]\n    },\n    \"GameServerData\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerData\"\n        },\n        {\n          \"description\": \"A set of custom game server properties, formatted as a single string value. This data is passed to a game client or service when it requests information on game servers. \"\n        }\n      ]\n    },\n    \"UtilizationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerUtilizationStatus\"\n        },\n        {\n          \"description\": \"Indicates whether the game server is available or is currently hosting gameplay.\"\n        }\n      ]\n    },\n    \"HealthCheck\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerHealthCheck\"\n        },\n        {\n          \"description\": \"Indicates health status of the game server. A request that includes this parameter updates the game server's <i>LastHealthCheckTime</i> timestamp. \"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"GameServerGroupName\",\n    \"GameServerId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-server-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateGameServerInput
---
