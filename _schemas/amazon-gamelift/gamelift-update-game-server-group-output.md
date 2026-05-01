---
description: UpdateGameServerGroupOutput schema from Amazon GameLift API
layout: schema
name: UpdateGameServerGroupOutput
properties_list:
- description: ''
  name: GameServerGroup
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-game-server-group-output-schema.json
slug: gamelift-update-game-server-group-output
source_filename: gamelift-update-game-server-group-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-server-group-output-schema.json\",\n  \"title\": \"UpdateGameServerGroupOutput\",\n  \"description\": \"UpdateGameServerGroupOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroup\"\n        },\n        {\n          \"description\": \"An object that describes the game server group resource with updated properties. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-server-group-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateGameServerGroupOutput
---
