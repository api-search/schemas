---
description: UpdateGameSessionInput schema from Amazon GameLift API
layout: schema
name: UpdateGameSessionInput
properties_list:
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: MaximumPlayerSessionCount
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PlayerSessionCreationPolicy
  type: object
- description: ''
  name: ProtectionPolicy
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-game-session-input-schema.json
slug: gamelift-update-game-session-input
source_filename: gamelift-update-game-session-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-session-input-schema.json\",\n  \"title\": \"UpdateGameSessionInput\",\n  \"description\": \"UpdateGameSessionInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session to update. \"\n        }\n      ]\n    },\n    \"MaximumPlayerSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of players that can be connected simultaneously to the game session.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a game session. Session names do not need to be unique.\"\n        }\n      ]\n    },\n    \"PlayerSessionCreationPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerSessionCreationPolicy\"\n        },\n        {\n          \"description\": \"A policy that determines whether the game session is accepting new players.\"\n        }\n      ]\n    },\n    \"ProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtectionPolicy\"\n        },\n        {\n          \"description\": \"<p>Game session protection policy to apply to this game session only.</p> <ul> <li> <p> <b>NoProtection</b> -- The game session can be terminated during a scale-down event.</p> </li> <li> <p> <b>FullProtection</b> -- If the game session is in an <code>ACTIVE</code>\
  \ status, it cannot be terminated during a scale-down event.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameSessionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-game-session-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateGameSessionInput
---
