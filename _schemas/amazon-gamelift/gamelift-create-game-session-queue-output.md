---
description: CreateGameSessionQueueOutput schema from Amazon GameLift API
layout: schema
name: CreateGameSessionQueueOutput
properties_list:
- description: ''
  name: GameSessionQueue
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-game-session-queue-output-schema.json
slug: gamelift-create-game-session-queue-output
source_filename: gamelift-create-game-session-queue-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-game-session-queue-output-schema.json\",\n  \"title\": \"CreateGameSessionQueueOutput\",\n  \"description\": \"CreateGameSessionQueueOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionQueue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueue\"\n        },\n        {\n          \"description\": \"An object that describes the newly created game session queue.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-game-session-queue-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateGameSessionQueueOutput
---
