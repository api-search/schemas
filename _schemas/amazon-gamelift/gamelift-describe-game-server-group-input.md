---
description: DescribeGameServerGroupInput schema from Amazon GameLift API
layout: schema
name: DescribeGameServerGroupInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-server-group-input-schema.json
slug: gamelift-describe-game-server-group-input
source_filename: gamelift-describe-game-server-group-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-group-input-schema.json\",\n  \"title\": \"DescribeGameServerGroupInput\",\n  \"description\": \"DescribeGameServerGroupInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group. Use either the name or ARN value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-group-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameServerGroupInput
---
