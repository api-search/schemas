---
description: StartGameSessionPlacementOutput schema from Amazon GameLift API
layout: schema
name: StartGameSessionPlacementOutput
properties_list:
- description: ''
  name: GameSessionPlacement
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-start-game-session-placement-output-schema.json
slug: gamelift-start-game-session-placement-output
source_filename: gamelift-start-game-session-placement-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-game-session-placement-output-schema.json\",\n  \"title\": \"StartGameSessionPlacementOutput\",\n  \"description\": \"StartGameSessionPlacementOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionPlacement\"\n        },\n        {\n          \"description\": \"Object that describes the newly created game session placement. This object includes all the information provided in the request, as well as start/end time stamps and placement status. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-game-session-placement-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StartGameSessionPlacementOutput
---
