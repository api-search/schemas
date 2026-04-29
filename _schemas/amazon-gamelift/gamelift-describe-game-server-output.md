---
description: DescribeGameServerOutput schema from Amazon GameLift API
layout: schema
name: DescribeGameServerOutput
properties_list:
- description: ''
  name: GameServer
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-server-output-schema.json
slug: gamelift-describe-game-server-output
source_filename: gamelift-describe-game-server-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-output-schema.json\",\n  \"title\": \"DescribeGameServerOutput\",\n  \"description\": \"DescribeGameServerOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServer\"\n        },\n        {\n          \"description\": \"Object that describes the requested game server.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameServerOutput
---
