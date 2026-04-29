---
description: A game session's properties plus the protection policy currently in force.
layout: schema
name: GameSessionDetail
properties_list:
- description: ''
  name: GameSession
  type: object
- description: ''
  name: ProtectionPolicy
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-session-detail-schema.json
slug: gamelift-game-session-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-detail-schema.json\",\n  \"title\": \"GameSessionDetail\",\n  \"description\": \"A game session's properties plus the protection policy currently in force.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSession\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSession\"\n        },\n        {\n          \"description\": \"Object that describes a game session.\"\n        }\n      ]\n    },\n    \"ProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtectionPolicy\"\n        },\n        {\n          \"description\": \"<p>Current status of protection for the game session.</p> <ul> <li> <p> <b>NoProtection</b> -- The game session can be terminated during a scale-down event.</p> </li> <li> <p>\
  \ <b>FullProtection</b> -- If the game session is in an <code>ACTIVE</code> status, it cannot be terminated during a scale-down event.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-detail-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameSessionDetail
---
