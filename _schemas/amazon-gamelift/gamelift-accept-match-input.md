---
description: AcceptMatchInput schema from Amazon GameLift API
layout: schema
name: AcceptMatchInput
properties_list:
- description: ''
  name: TicketId
  type: object
- description: ''
  name: PlayerIds
  type: object
- description: ''
  name: AcceptanceType
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-accept-match-input-schema.json
slug: gamelift-accept-match-input
source_filename: gamelift-accept-match-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-accept-match-input-schema.json\",\n  \"title\": \"AcceptMatchInput\",\n  \"description\": \"AcceptMatchInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a matchmaking ticket. The ticket must be in status <code>REQUIRES_ACCEPTANCE</code>; otherwise this request will fail.\"\n        }\n      ]\n    },\n    \"PlayerIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"A unique identifier for a player delivering the response. This parameter can include one or multiple player\
  \ IDs.\"\n        }\n      ]\n    },\n    \"AcceptanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AcceptanceType\"\n        },\n        {\n          \"description\": \"Player response to the proposed match.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TicketId\",\n    \"PlayerIds\",\n    \"AcceptanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-accept-match-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: AcceptMatchInput
---
