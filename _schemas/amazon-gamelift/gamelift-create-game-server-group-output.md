---
description: CreateGameServerGroupOutput schema from Amazon GameLift API
layout: schema
name: CreateGameServerGroupOutput
properties_list:
- description: ''
  name: GameServerGroup
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-game-server-group-output-schema.json
slug: gamelift-create-game-server-group-output
source_filename: gamelift-create-game-server-group-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-game-server-group-output-schema.json\",\n  \"title\": \"CreateGameServerGroupOutput\",\n  \"description\": \"CreateGameServerGroupOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroup\"\n        },\n        {\n          \"description\": \"The newly created game server group object, including the new ARN value for the Amazon GameLift FleetIQ game server group and the object's status. The Amazon EC2 Auto Scaling group ARN is initially null, since the group has not yet been created. This value is added once the game server group status reaches <code>ACTIVE</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-game-server-group-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateGameServerGroupOutput
---
