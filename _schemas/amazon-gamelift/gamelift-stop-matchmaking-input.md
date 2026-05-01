---
description: StopMatchmakingInput schema from Amazon GameLift API
layout: schema
name: StopMatchmakingInput
properties_list:
- description: ''
  name: TicketId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-stop-matchmaking-input-schema.json
slug: gamelift-stop-matchmaking-input
source_filename: gamelift-stop-matchmaking-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-matchmaking-input-schema.json\",\n  \"title\": \"StopMatchmakingInput\",\n  \"description\": \"StopMatchmakingInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a matchmaking ticket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TicketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-matchmaking-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StopMatchmakingInput
---
