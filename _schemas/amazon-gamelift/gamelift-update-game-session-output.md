---
description: UpdateGameSessionOutput schema from Amazon GameLift API
layout: schema
name: UpdateGameSessionOutput
properties_list:
- description: ''
  name: GameSession
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-game-session-output-schema.json
slug: gamelift-update-game-session-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-session-output-schema.json\",\n  \"title\": \"UpdateGameSessionOutput\",\n  \"description\": \"UpdateGameSessionOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSession\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSession\"\n        },\n        {\n          \"description\": \"The updated game session properties.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-session-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateGameSessionOutput
---
