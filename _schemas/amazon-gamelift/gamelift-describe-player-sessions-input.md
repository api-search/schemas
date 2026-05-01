---
description: DescribePlayerSessionsInput schema from Amazon GameLift API
layout: schema
name: DescribePlayerSessionsInput
properties_list:
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: PlayerSessionId
  type: object
- description: ''
  name: PlayerSessionStatusFilter
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-player-sessions-input-schema.json
slug: gamelift-describe-player-sessions-input
source_filename: gamelift-describe-player-sessions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-player-sessions-input-schema.json\",\n  \"title\": \"DescribePlayerSessionsInput\",\n  \"description\": \"DescribePlayerSessionsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session to retrieve player sessions for.\"\n        }\n      ]\n    },\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player to retrieve player sessions for.\"\n        }\n      ]\n    },\n    \"PlayerSessionId\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerSessionId\"\n        },\n        {\n          \"description\": \"A unique identifier for a player session to retrieve.\"\n        }\n      ]\n    },\n    \"PlayerSessionStatusFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"<p>Player session status to filter results on. Note that when a PlayerSessionId or PlayerId is provided in a DescribePlayerSessions request, then the PlayerSessionStatusFilter has no effect on the response.</p> <p>Possible player session statuses include the following:</p> <ul> <li> <p> <b>RESERVED</b> -- The player session request has been received, but the player has not yet connected to the server process and/or been validated. </p> </li> <li> <p> <b>ACTIVE</b> -- The player has been validated by the server process and is currently connected.</p> </li> <li> <p> <b>COMPLETED</b> --\
  \ The player connection has been dropped.</p> </li> <li> <p> <b>TIMEDOUT</b> -- A player session request was received, but the player did not connect and/or was not validated within the timeout limit (60 seconds).</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages. If a player session ID is specified, this parameter is ignored.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the\
  \ result set, do not specify a value. If a player session ID is specified, this parameter is ignored.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-player-sessions-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribePlayerSessionsInput
---
