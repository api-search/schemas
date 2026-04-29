---
description: StartMatchmakingOutput schema from Amazon GameLift API
layout: schema
name: StartMatchmakingOutput
properties_list:
- description: ''
  name: MatchmakingTicket
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-start-matchmaking-output-schema.json
slug: gamelift-start-matchmaking-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-matchmaking-output-schema.json\",\n  \"title\": \"StartMatchmakingOutput\",\n  \"description\": \"StartMatchmakingOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MatchmakingTicket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingTicket\"\n        },\n        {\n          \"description\": \"Ticket representing the matchmaking request. This object include the information included in the request, ticket status, and match results as generated during the matchmaking process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-matchmaking-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StartMatchmakingOutput
---
