---
description: StartGameSessionPlacementInput schema from Amazon GameLift API
layout: schema
name: StartGameSessionPlacementInput
properties_list:
- description: ''
  name: PlacementId
  type: object
- description: ''
  name: GameSessionQueueName
  type: object
- description: ''
  name: GameProperties
  type: object
- description: ''
  name: MaximumPlayerSessionCount
  type: object
- description: ''
  name: GameSessionName
  type: object
- description: ''
  name: PlayerLatencies
  type: object
- description: ''
  name: DesiredPlayerSessions
  type: object
- description: ''
  name: GameSessionData
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-start-game-session-placement-input-schema.json
slug: gamelift-start-game-session-placement-input
source_filename: gamelift-start-game-session-placement-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-game-session-placement-input-schema.json\",\n  \"title\": \"StartGameSessionPlacementInput\",\n  \"description\": \"StartGameSessionPlacementInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlacementId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier to assign to the new game session placement. This value is developer-defined. The value must be unique across all Regions and cannot be reused.\"\n        }\n      ]\n    },\n    \"GameSessionQueueName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueueNameOrArn\"\n        },\n        {\n          \"description\": \"Name of the queue to\
  \ use to place the new game session. You can use either the queue name or ARN value. \"\n        }\n      ]\n    },\n    \"GameProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GamePropertyList\"\n        },\n        {\n          \"description\": \"A set of custom properties for a game session, formatted as key:value pairs. These properties are passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"MaximumPlayerSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of players that can be connected simultaneously to the game session.\"\n        }\n      ]\n    },\n    \"GameSessionName\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a game session. Session names do not need to be unique.\"\n        }\n      ]\n    },\n    \"PlayerLatencies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerLatencyList\"\n        },\n        {\n          \"description\": \"A set of values, expressed in milliseconds, that indicates the amount of latency that a player experiences when connected to Amazon Web Services Regions. This information is used to try to place the new game session where it can offer the best possible gameplay experience for the players. \"\n        }\n      ]\n    },\n    \"DesiredPlayerSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredPlayerSessionList\"\n        },\n        {\n          \"description\": \"Set of information on each player to create a player\
  \ session for.\"\n        }\n      ]\n    },\n    \"GameSessionData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LargeGameSessionData\"\n        },\n        {\n          \"description\": \"A set of custom game session properties, formatted as a single string value. This data is passed to a game server process in the <code>GameSession</code> object with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PlacementId\",\n    \"GameSessionQueueName\",\n    \"MaximumPlayerSessionCount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-game-session-placement-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StartGameSessionPlacementInput
---
