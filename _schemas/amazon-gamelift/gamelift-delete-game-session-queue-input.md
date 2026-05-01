---
description: DeleteGameSessionQueueInput schema from Amazon GameLift API
layout: schema
name: DeleteGameSessionQueueInput
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-game-session-queue-input-schema.json
slug: gamelift-delete-game-session-queue-input
source_filename: gamelift-delete-game-session-queue-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-game-session-queue-input-schema.json\",\n  \"title\": \"DeleteGameSessionQueueInput\",\n  \"description\": \"DeleteGameSessionQueueInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueueNameOrArn\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with game session queue. Queue names must be unique within each Region. You can use either the queue ID or ARN value. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-game-session-queue-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteGameSessionQueueInput
---
