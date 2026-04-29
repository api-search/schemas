---
description: StopGameSessionPlacementInput schema from Amazon GameLift API
layout: schema
name: StopGameSessionPlacementInput
properties_list:
- description: ''
  name: PlacementId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-stop-game-session-placement-input-schema.json
slug: gamelift-stop-game-session-placement-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-game-session-placement-input-schema.json\",\n  \"title\": \"StopGameSessionPlacementInput\",\n  \"description\": \"StopGameSessionPlacementInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlacementId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a game session placement to stop.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PlacementId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-game-session-placement-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StopGameSessionPlacementInput
---
