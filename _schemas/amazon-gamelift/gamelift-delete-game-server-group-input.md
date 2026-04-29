---
description: DeleteGameServerGroupInput schema from Amazon GameLift API
layout: schema
name: DeleteGameServerGroupInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: DeleteOption
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-game-server-group-input-schema.json
slug: gamelift-delete-game-server-group-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-game-server-group-input-schema.json\",\n  \"title\": \"DeleteGameServerGroupInput\",\n  \"description\": \"DeleteGameServerGroupInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group. Use either the name or ARN value.\"\n        }\n      ]\n    },\n    \"DeleteOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupDeleteOption\"\n        },\n        {\n          \"description\": \"<p>The type of delete to perform. Options include the following:</p> <ul> <li> <p> <code>SAFE_DELETE</code>\
  \ \\u2013 (default) Terminates the game server group and Amazon EC2 Auto Scaling group only when it has no game servers that are in <code>UTILIZED</code> status.</p> </li> <li> <p> <code>FORCE_DELETE</code> \\u2013 Terminates the game server group, including all active game servers regardless of their utilization status, and the Amazon EC2 Auto Scaling group. </p> </li> <li> <p> <code>RETAIN</code> \\u2013 Does a safe delete of the game server group but retains the Amazon EC2 Auto Scaling group as is.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-game-server-group-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteGameServerGroupInput
---
