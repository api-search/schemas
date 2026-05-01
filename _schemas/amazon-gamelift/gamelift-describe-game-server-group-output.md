---
description: DescribeGameServerGroupOutput schema from Amazon GameLift API
layout: schema
name: DescribeGameServerGroupOutput
properties_list:
- description: ''
  name: GameServerGroup
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-server-group-output-schema.json
slug: gamelift-describe-game-server-group-output
source_filename: gamelift-describe-game-server-group-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-group-output-schema.json\",\n  \"title\": \"DescribeGameServerGroupOutput\",\n  \"description\": \"DescribeGameServerGroupOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroup\"\n        },\n        {\n          \"description\": \"An object with the property settings for the requested game server group resource. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-group-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameServerGroupOutput
---
