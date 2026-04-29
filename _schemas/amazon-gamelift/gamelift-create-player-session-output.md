---
description: CreatePlayerSessionOutput schema from Amazon GameLift API
layout: schema
name: CreatePlayerSessionOutput
properties_list:
- description: ''
  name: PlayerSession
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-player-session-output-schema.json
slug: gamelift-create-player-session-output
source_filename: gamelift-create-player-session-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-session-output-schema.json\",\n  \"title\": \"CreatePlayerSessionOutput\",\n  \"description\": \"CreatePlayerSessionOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerSession\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerSession\"\n        },\n        {\n          \"description\": \"Object that describes the newly created player session record.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-player-session-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreatePlayerSessionOutput
---
