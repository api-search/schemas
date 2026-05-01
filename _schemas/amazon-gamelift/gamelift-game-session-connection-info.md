---
description: Connection information for a new game session that is created in response to a start matchmaking request. Once a match is made, the FlexMatch engine creates a new game session for it. This information, including the game session endpoint and player sessions for each player in the original matchmaking request, is added to the matchmaking ticket.
layout: schema
name: GameSessionConnectionInfo
properties_list:
- description: ''
  name: GameSessionArn
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
  name: MatchedPlayerSessions
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-game-session-connection-info-schema.json
slug: gamelift-game-session-connection-info
source_filename: gamelift-game-session-connection-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-connection-info-schema.json\",\n  \"title\": \"GameSessionConnectionInfo\",\n  \"description\": \"Connection information for a new game session that is created in response to a start matchmaking request. Once a match is made, the FlexMatch engine creates a new game session for it. This information, including the game session endpoint and player sessions for each player in the original matchmaking request, is added to the matchmaking ticket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session. Use the game session ID.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the game session. To connect to a Amazon GameLift game server, an app needs both the IP address and port number.\"\n        }\n      ]\n    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsName\"\n        },\n        {\n          \"description\": \"<p>The DNS identifier assigned to the instance that is running the game session. Values have the following format:</p> <ul> <li> <p>TLS-enabled fleets: <code>&lt;unique identifier&gt;.&lt;region identifier&gt;.amazongamelift.com</code>.</p> </li> <li> <p>Non-TLS-enabled fleets: <code>ec2-&lt;unique identifier&gt;.compute.amazonaws.com</code>. (See <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-instance-addressing.html#concepts-public-addresses\\\">Amazon EC2 Instance IP Addressing</a>.)</p> </li> </ul> <p>When connecting\
  \ to a game session that is running on a TLS-enabled fleet, you must use the DNS name, not the IP address.</p>\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The port number for the game session. To connect to a Amazon GameLift game server, an app needs both the IP address and port number.\"\n        }\n      ]\n    },\n    \"MatchedPlayerSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchedPlayerSessionList\"\n        },\n        {\n          \"description\": \"A collection of player session IDs, one for each player ID that was included in the original matchmaking request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-game-session-connection-info-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GameSessionConnectionInfo
---
