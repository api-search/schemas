---
description: StopGameSessionPlacementOutput schema from Amazon GameLift API
layout: schema
name: StopGameSessionPlacementOutput
properties_list:
- description: ''
  name: GameSessionPlacement
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-stop-game-session-placement-output-schema.json
slug: gamelift-stop-game-session-placement-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-game-session-placement-output-schema.json\",\n  \"title\": \"StopGameSessionPlacementOutput\",\n  \"description\": \"StopGameSessionPlacementOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionPlacement\"\n        },\n        {\n          \"description\": \"Object that describes the canceled game session placement, with <code>CANCELLED</code> status and an end time stamp. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-game-session-placement-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StopGameSessionPlacementOutput
---
