---
description: RegisterGameServerInput schema from Amazon GameLift API
layout: schema
name: RegisterGameServerInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: GameServerId
  type: object
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: ConnectionInfo
  type: object
- description: ''
  name: GameServerData
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-register-game-server-input-schema.json
slug: gamelift-register-game-server-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-register-game-server-input-schema.json\",\n  \"title\": \"RegisterGameServerInput\",\n  \"description\": \"RegisterGameServerInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group where the game server is running.\"\n        }\n      ]\n    },\n    \"GameServerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerId\"\n        },\n        {\n          \"description\": \"A custom string that uniquely identifies the game server to register. Game server IDs are developer-defined and must be unique\
  \ across all game server groups in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerInstanceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the instance where the game server is running. This ID is available in the instance metadata. EC2 instance IDs use a 17-character format, for example: <code>i-1234567890abcdef0</code>.\"\n        }\n      ]\n    },\n    \"ConnectionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerConnectionInfo\"\n        },\n        {\n          \"description\": \"Information that is needed to make inbound client connections to the game server. This might include the IP address and port, DNS name, and other information.\"\n        }\n      ]\n    },\n    \"GameServerData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerData\"\
  \n        },\n        {\n          \"description\": \"A set of custom game server properties, formatted as a single string value. This data is passed to a game client or service when it requests information on game servers. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\",\n    \"GameServerId\",\n    \"InstanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-register-game-server-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: RegisterGameServerInput
---
