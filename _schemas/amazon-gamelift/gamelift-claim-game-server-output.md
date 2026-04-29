---
description: ClaimGameServerOutput schema from Amazon GameLift API
layout: schema
name: ClaimGameServerOutput
properties_list:
- description: ''
  name: GameServer
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-claim-game-server-output-schema.json
slug: gamelift-claim-game-server-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-claim-game-server-output-schema.json\",\n  \"title\": \"ClaimGameServerOutput\",\n  \"description\": \"ClaimGameServerOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServer\"\n        },\n        {\n          \"description\": \"Object that describes the newly claimed game server.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-claim-game-server-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ClaimGameServerOutput
---
