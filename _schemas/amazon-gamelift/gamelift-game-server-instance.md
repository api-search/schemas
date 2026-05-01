---
description: <p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p> Additional properties, including status, that describe an EC2 instance in a game server group. Instance configurations are set with game server group properties (see <code>DescribeGameServerGroup</code> and with the EC2 launch template that was used when creating the game server group. </p> <p>Retrieve game server instances for a game server group by calling <code>DescribeGameServerInstances</code>. </p>
layout: schema
name: GameServerInstance
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: GameServerGroupArn
  type: object
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: InstanceStatus
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-server-instance-schema.json
slug: gamelift-game-server-instance
source_filename: gamelift-game-server-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-instance-schema.json\",\n  \"title\": \"GameServerInstance\",\n  \"description\": \"<p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p> Additional properties, including status, that describe an EC2 instance in a game server group. Instance configurations are set with game server group properties (see <code>DescribeGameServerGroup</code> and with the EC2 launch template that was used when creating the game server group. </p> <p>Retrieve game server instances for a game server group by calling <code>DescribeGameServerInstances</code>. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupName\"\n        },\n        {\n\
  \          \"description\": \"A developer-defined identifier for the game server group that includes the game server instance. The name is unique for each Region in each Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"GameServerGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupArn\"\n        },\n        {\n          \"description\": \"A generated unique identifier for the game server group that includes the game server instance. \"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerInstanceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the instance where the game server is running. This ID is available in the instance metadata. EC2 instance IDs use a 17-character format, for example: <code>i-1234567890abcdef0</code>.\"\n        }\n      ]\n    },\n    \"InstanceStatus\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/GameServerInstanceStatus\"\n        },\n        {\n          \"description\": \"Current status of the game server instance\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-server-instance-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameServerInstance
---
