---
description: <p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Properties describing a game server that is running on an instance in a game server group. </p> <p>A game server is created by a successful call to <code>RegisterGameServer</code> and deleted by calling <code>DeregisterGameServer</code>. A game server is claimed to host a game session by calling <code>ClaimGameServer</code>. </p>
layout: schema
name: GameServer
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: GameServerGroupArn
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
- description: ''
  name: ClaimStatus
  type: object
- description: ''
  name: UtilizationStatus
  type: object
- description: ''
  name: RegistrationTime
  type: object
- description: ''
  name: LastClaimTime
  type: object
- description: ''
  name: LastHealthCheckTime
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-server-schema.json
slug: gamelift-game-server
source_filename: gamelift-game-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-schema.json\",\n  \"title\": \"GameServer\",\n  \"description\": \"<p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>Properties describing a game server that is running on an instance in a game server group. </p> <p>A game server is created by a successful call to <code>RegisterGameServer</code> and deleted by calling <code>DeregisterGameServer</code>. A game server is claimed to host a game session by calling <code>ClaimGameServer</code>. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupName\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group where the game server\
  \ is running.\"\n        }\n      ]\n    },\n    \"GameServerGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupArn\"\n        },\n        {\n          \"description\": \"The ARN identifier for the game server group where the game server is located.\"\n        }\n      ]\n    },\n    \"GameServerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerId\"\n        },\n        {\n          \"description\": \"A custom string that uniquely identifies the game server. Game server IDs are developer-defined and are unique across all game server groups in an Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerInstanceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the instance where the game server is running. This ID is available in the instance metadata.\
  \ EC2 instance IDs use a 17-character format, for example: <code>i-1234567890abcdef0</code>.\"\n        }\n      ]\n    },\n    \"ConnectionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerConnectionInfo\"\n        },\n        {\n          \"description\": \"The port and IP address that must be used to establish a client connection to the game server.\"\n        }\n      ]\n    },\n    \"GameServerData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerData\"\n        },\n        {\n          \"description\": \"A set of custom game server properties, formatted as a single string value. This data is passed to a game client or service when it requests information on game servers.\"\n        }\n      ]\n    },\n    \"ClaimStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerClaimStatus\"\n        },\n        {\n          \"description\": \"Indicates when an available\
  \ game server has been reserved for gameplay but has not yet started hosting a game. Once it is claimed, the game server remains in <code>CLAIMED</code> status for a maximum of one minute. During this time, game clients connect to the game server to start the game and trigger the game server to update its utilization status. After one minute, the game server claim status reverts to null.\"\n        }\n      ]\n    },\n    \"UtilizationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerUtilizationStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the game server is currently available for new games or is busy. Possible statuses include:</p> <ul> <li> <p> <code>AVAILABLE</code> - The game server is available to be claimed. A game server that has been claimed remains in this status until it reports game hosting activity. </p> </li> <li> <p> <code>UTILIZED</code> - The game server is currently hosting a game session\
  \ with players. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"RegistrationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Timestamp that indicates when the game server registered. The format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"LastClaimTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Timestamp that indicates the last time the game server was claimed. The format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>). This value is used to calculate when a claimed game server's status should revert to null.\"\n        }\n      ]\n    },\n    \"LastHealthCheckTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"Timestamp that indicates the last time the game server was updated with health status. The format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>). After game server registration, this property is only changed when a game server update specifies a health check value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameServer
---
