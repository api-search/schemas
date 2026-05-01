---
description: This object includes the full details of the original request plus the current status and start/end time stamps.
layout: schema
name: GameSessionPlacement
properties_list:
- description: ''
  name: PlacementId
  type: object
- description: ''
  name: GameSessionQueueName
  type: object
- description: ''
  name: Status
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
  name: GameSessionId
  type: object
- description: ''
  name: GameSessionArn
  type: object
- description: ''
  name: GameSessionRegion
  type: object
- description: ''
  name: PlayerLatencies
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
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
  name: PlacedPlayerSessions
  type: object
- description: ''
  name: GameSessionData
  type: object
- description: ''
  name: MatchmakerData
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-session-placement-schema.json
slug: gamelift-game-session-placement
source_filename: gamelift-game-session-placement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-placement-schema.json\",\n  \"title\": \"GameSessionPlacement\",\n  \"description\": \"This object includes the full details of the original request plus the current status and start/end time stamps.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlacementId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a game session placement.\"\n        }\n      ]\n    },\n    \"GameSessionQueueName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionQueueName\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with game session queue. Queue names must be unique within each Region.\"\
  \n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionPlacementState\"\n        },\n        {\n          \"description\": \"<p>Current status of the game session placement request.</p> <ul> <li> <p> <b>PENDING</b> -- The placement request is currently in the queue waiting to be processed.</p> </li> <li> <p> <b>FULFILLED</b> -- A new game session and player sessions (if requested) have been successfully created. Values for <i>GameSessionArn</i> and <i>GameSessionRegion</i> are available. </p> </li> <li> <p> <b>CANCELLED</b> -- The placement request was canceled.</p> </li> <li> <p> <b>TIMED_OUT</b> -- A new game session was not successfully created before the time limit expired. You can resubmit the placement request as needed.</p> </li> <li> <p> <b>FAILED</b> -- Amazon GameLift is not able to complete the process of placing the game session. Common reasons are the game session terminated before the placement\
  \ process was completed, or an unexpected internal error.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"GameProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GamePropertyList\"\n        },\n        {\n          \"description\": \"A set of custom properties for a game session, formatted as key:value pairs. These properties are passed to a game server process with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"MaximumPlayerSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of players that can be connected simultaneously to the game session.\"\n        }\n      ]\n    },\n    \"GameSessionName\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a game session. Session names do not need to be unique.\"\n        }\n      ]\n    },\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session. This value is set once the new game session is placed (placement status is <code>FULFILLED</code>).\"\n        }\n      ]\n    },\n    \"GameSessionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Identifier for the game session created by this placement request. This value is set once the new game session is placed (placement status is <code>FULFILLED</code>). This identifier is unique across all Regions. You\
  \ can use this value as a <code>GameSessionId</code> value as needed.\"\n        }\n      ]\n    },\n    \"GameSessionRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Name of the Region where the game session created by this placement request is running. This value is set once the new game session is placed (placement status is <code>FULFILLED</code>).\"\n        }\n      ]\n    },\n    \"PlayerLatencies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerLatencyList\"\n        },\n        {\n          \"description\": \"A set of values, expressed in milliseconds, that indicates the amount of latency that a player experiences when connected to Amazon Web Services Regions.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n        \
  \  \"description\": \"Time stamp indicating when this request was placed in the queue. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time stamp indicating when this request was completed, canceled, or timed out.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the game session. To connect to a Amazon GameLift game server, an app needs both the IP address and port number. This value is set once the new game session is placed (placement status is <code>FULFILLED</code>). \"\n        }\n      ]\n    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsName\"\
  \n        },\n        {\n          \"description\": \"<p>The DNS identifier assigned to the instance that is running the game session. Values have the following format:</p> <ul> <li> <p>TLS-enabled fleets: <code>&lt;unique identifier&gt;.&lt;region identifier&gt;.amazongamelift.com</code>.</p> </li> <li> <p>Non-TLS-enabled fleets: <code>ec2-&lt;unique identifier&gt;.compute.amazonaws.com</code>. (See <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-instance-addressing.html#concepts-public-addresses\\\">Amazon EC2 Instance IP Addressing</a>.)</p> </li> </ul> <p>When connecting to a game session that is running on a TLS-enabled fleet, you must use the DNS name, not the IP address.</p>\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The port number for the game session. To connect to a Amazon GameLift game server, an app needs both\
  \ the IP address and port number. This value is set once the new game session is placed (placement status is <code>FULFILLED</code>).\"\n        }\n      ]\n    },\n    \"PlacedPlayerSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacedPlayerSessionList\"\n        },\n        {\n          \"description\": \"A collection of information on player sessions created in response to the game session placement request. These player sessions are created only once a new game session is successfully placed (placement status is <code>FULFILLED</code>). This information includes the player ID (as provided in the placement request) and the corresponding player session ID.\"\n        }\n      ]\n    },\n    \"GameSessionData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LargeGameSessionData\"\n        },\n        {\n          \"description\": \"A set of custom game session properties, formatted as a single string value. This\
  \ data is passed to a game server process in the <code>GameSession</code> object with a request to start a new game session (see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-startsession\\\">Start a Game Session</a>).\"\n        }\n      ]\n    },\n    \"MatchmakerData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakerData\"\n        },\n        {\n          \"description\": \"Information on the matchmaking process for this game. Data is in JSON syntax, formatted as a string. It identifies the matchmaking configuration used to create the match, and contains data on all players assigned to the match, including player attributes and team assignments. For more details on matchmaker data, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-server.html#match-server-data\\\">Match Data</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-placement-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameSessionPlacement
---
