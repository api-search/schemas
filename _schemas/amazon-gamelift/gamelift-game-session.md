---
description: <p>Properties describing a game session.</p> <p>A game session in ACTIVE status can host players. When a game session ends, its status is set to <code>TERMINATED</code>. </p> <p>Once the session ends, the game session object is retained for 30 days. This means you can reuse idempotency token values after this time. Game session logs are retained for 14 days.</p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: GameSession
properties_list:
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: TerminationTime
  type: object
- description: ''
  name: CurrentPlayerSessionCount
  type: object
- description: ''
  name: MaximumPlayerSessionCount
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusReason
  type: object
- description: ''
  name: GameProperties
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: DnsName
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: PlayerSessionCreationPolicy
  type: object
- description: ''
  name: CreatorId
  type: object
- description: ''
  name: GameSessionData
  type: object
- description: ''
  name: MatchmakerData
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-session-schema.json
slug: gamelift-game-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-schema.json\",\n  \"title\": \"GameSession\",\n  \"description\": \"<p>Properties describing a game session.</p> <p>A game session in ACTIVE status can host players. When a game session ends, its status is set to <code>TERMINATED</code>. </p> <p>Once the session ends, the game session object is retained for 30 days. This means you can reuse idempotency token values after this time. Game session logs are retained for 14 days.</p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n\
  \          \"description\": \"A unique identifier for the game session. A game session ARN has the following format: <code>arn:aws:gamelift:&lt;region&gt;::gamesession/&lt;fleet ID&gt;/&lt;custom ID string or idempotency token&gt;</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a game session. Session names do not need to be unique.\"\n        }\n      ]\n    },\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that the game session is running on.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource\
  \ Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) associated with the GameLift fleet that this game session is running on. \"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"TerminationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was terminated. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"CurrentPlayerSessionCount\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"Number of players currently in the game session.\"\n        }\n      ]\n    },\n    \"MaximumPlayerSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of players that can be connected simultaneously to the game session.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionStatus\"\n        },\n        {\n          \"description\": \"Current status of the game session. A game session must have an <code>ACTIVE</code> status to have player sessions.\"\n        }\n      ]\n    },\n    \"StatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionStatusReason\"\n        },\n        {\n          \"description\": \"Provides additional\
  \ information about game session status. <code>INTERRUPTED</code> indicates that the game session was hosted on a spot instance that was reclaimed, causing the active game session to be terminated.\"\n        }\n      ]\n    },\n    \"GameProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GamePropertyList\"\n        },\n        {\n          \"description\": \"A set of custom properties for a game session, formatted as key:value pairs. These properties are passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the game session. To connect to a Amazon GameLift\
  \ game server, an app needs both the IP address and port number.\"\n        }\n      ]\n    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsName\"\n        },\n        {\n          \"description\": \"<p>The DNS identifier assigned to the instance that is running the game session. Values have the following format:</p> <ul> <li> <p>TLS-enabled fleets: <code>&lt;unique identifier&gt;.&lt;region identifier&gt;.amazongamelift.com</code>.</p> </li> <li> <p>Non-TLS-enabled fleets: <code>ec2-&lt;unique identifier&gt;.compute.amazonaws.com</code>. (See <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-instance-addressing.html#concepts-public-addresses\\\">Amazon EC2 Instance IP Addressing</a>.)</p> </li> </ul> <p>When connecting to a game session that is running on a TLS-enabled fleet, you must use the DNS name, not the IP address.</p>\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The port number for the game session. To connect to a Amazon GameLift game server, an app needs both the IP address and port number.\"\n        }\n      ]\n    },\n    \"PlayerSessionCreationPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerSessionCreationPolicy\"\n        },\n        {\n          \"description\": \"Indicates whether or not the game session is accepting new players.\"\n        }\n      ]\n    },\n    \"CreatorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player. This ID is used to enforce a resource protection policy (if one exists), that limits the number of game sessions a player can create.\"\n        }\n      ]\n    },\n    \"GameSessionData\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/LargeGameSessionData\"\n        },\n        {\n          \"description\": \"A set of custom game session properties, formatted as a single string value. This data is passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"MatchmakerData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakerData\"\n        },\n        {\n          \"description\": \"Information about the matchmaking process that was used to create the game session. It is in JSON syntax, formatted as a string. In addition the matchmaking configuration used, it contains data on all players assigned to the match, including player attributes and team assignments. For more details on matchmaker data, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-server.html#match-server-data\\\
  \">Match Data</a>. Matchmaker data is useful when requesting match backfills, and is updated whenever new players are added during a successful backfill (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_StartMatchBackfill.html\\\">StartMatchBackfill</a>). \"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The fleet location where the game session is running. This value might specify the fleet's home Region or a remote location. Location is expressed as an Amazon Web Services Region code such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameSession
---
