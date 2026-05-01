---
description: CreateGameSessionInput schema from Amazon GameLift API
layout: schema
name: CreateGameSessionInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: AliasId
  type: object
- description: ''
  name: MaximumPlayerSessionCount
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: GameProperties
  type: object
- description: ''
  name: CreatorId
  type: object
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: IdempotencyToken
  type: object
- description: ''
  name: GameSessionData
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-game-session-input-schema.json
slug: gamelift-create-game-session-input
source_filename: gamelift-create-game-session-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-game-session-input-schema.json\",\n  \"title\": \"CreateGameSessionInput\",\n  \"description\": \"CreateGameSessionInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to create a game session in. You can use either the fleet ID or ARN value. Each request must reference either a fleet ID or alias ID, but not both.\"\n        }\n      ]\n    },\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the alias associated with the fleet\
  \ to create a game session in. You can use either the alias ID or ARN value. Each request must reference either a fleet ID or alias ID, but not both.\"\n        }\n      ]\n    },\n    \"MaximumPlayerSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of players that can be connected simultaneously to the game session.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a game session. Session names do not need to be unique.\"\n        }\n      ]\n    },\n    \"GameProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GamePropertyList\"\n        },\n        {\n          \"description\": \"A set of custom properties for a game session, formatted\
  \ as key:value pairs. These properties are passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"CreatorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"<p>A unique identifier for a player or entity creating the game session. </p> <p>If you add a resource creation limit policy to a fleet, the <code>CreateGameSession</code> operation requires a <code>CreatorId</code>. Amazon GameLift limits the number of game session creation requests with the same <code>CreatorId</code> in a specified time period.</p> <p>If you your fleet doesn't have a resource creation limit policy and you provide a <code>CreatorId</code> in your <code>CreateGameSession</code> requests,\
  \ Amazon GameLift limits requests to one request per <code>CreatorId</code> per second.</p> <p>To not limit <code>CreateGameSession</code> requests with the same <code>CreatorId</code>, don't provide a <code>CreatorId</code> in your <code>CreateGameSession</code> request.</p>\"\n        }\n      ]\n    },\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdStringModel\"\n        },\n        {\n          \"description\": \"<p> <i>This parameter is deprecated. Use <code>IdempotencyToken</code> instead.</i> </p> <p>Custom string that uniquely identifies a request for a new game session. Maximum token length is 48 characters. If provided, this string is included in the new game session's ID.</p>\"\n        }\n      ]\n    },\n    \"IdempotencyToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdStringModel\"\n        },\n        {\n          \"description\": \"Custom string that uniquely identifies the new\
  \ game session request. This is useful for ensuring that game session requests with the same idempotency token are processed only once. Subsequent requests with the same string return the original <code>GameSession</code> object, with an updated status. Maximum token length is 48 characters. If provided, this string is included in the new game session's ID. A game session ARN has the following format: <code>arn:aws:gamelift:&lt;region&gt;::gamesession/&lt;fleet ID&gt;/&lt;custom ID string or idempotency token&gt;</code>. Idempotency tokens remain in use for 30 days after a game session has ended; game session objects are retained for this time period and then deleted.\"\n        }\n      ]\n    },\n    \"GameSessionData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LargeGameSessionData\"\n        },\n        {\n          \"description\": \"A set of custom game session properties, formatted as a single string value. This data is passed to a game server\
  \ process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"A fleet's remote location to place the new game session in. If this parameter is not set, the new game session is placed in the fleet's home Region. Specify a remote location with an Amazon Web Services Region code such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaximumPlayerSessionCount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-game-session-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateGameSessionInput
---
