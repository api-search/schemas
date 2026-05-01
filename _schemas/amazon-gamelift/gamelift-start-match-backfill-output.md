---
description: StartMatchBackfillOutput schema from Amazon GameLift API
layout: schema
name: StartMatchBackfillOutput
properties_list:
- description: ''
  name: MatchmakingTicket
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-start-match-backfill-output-schema.json
slug: gamelift-start-match-backfill-output
source_filename: gamelift-start-match-backfill-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-match-backfill-output-schema.json\",\n  \"title\": \"StartMatchBackfillOutput\",\n  \"description\": \"StartMatchBackfillOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MatchmakingTicket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingTicket\"\n        },\n        {\n          \"description\": \"Ticket representing the backfill matchmaking request. This object includes the information in the request, ticket status, and match results as generated during the matchmaking process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-match-backfill-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StartMatchBackfillOutput
---
