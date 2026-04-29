---
description: DescribeGameSessionPlacementOutput schema from Amazon GameLift API
layout: schema
name: DescribeGameSessionPlacementOutput
properties_list:
- description: ''
  name: GameSessionPlacement
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-session-placement-output-schema.json
slug: gamelift-describe-game-session-placement-output
source_filename: gamelift-describe-game-session-placement-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-session-placement-output-schema.json\",\n  \"title\": \"DescribeGameSessionPlacementOutput\",\n  \"description\": \"DescribeGameSessionPlacementOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionPlacement\"\n        },\n        {\n          \"description\": \"Object that describes the requested game session placement.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-session-placement-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameSessionPlacementOutput
---
