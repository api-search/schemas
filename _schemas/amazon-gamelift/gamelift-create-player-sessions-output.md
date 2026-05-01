---
description: CreatePlayerSessionsOutput schema from Amazon GameLift API
layout: schema
name: CreatePlayerSessionsOutput
properties_list:
- description: ''
  name: PlayerSessions
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-player-sessions-output-schema.json
slug: gamelift-create-player-sessions-output
source_filename: gamelift-create-player-sessions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-sessions-output-schema.json\",\n  \"title\": \"CreatePlayerSessionsOutput\",\n  \"description\": \"CreatePlayerSessionsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerSessionList\"\n        },\n        {\n          \"description\": \"A collection of player session objects created for the added players.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-sessions-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreatePlayerSessionsOutput
---
