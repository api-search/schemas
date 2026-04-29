---
description: Information about a player session. This object contains only the player ID and player session ID. To retrieve full details on a player session, call <a href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribePlayerSessions.html">DescribePlayerSessions</a> with the player session ID.
layout: schema
name: PlacedPlayerSession
properties_list:
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: PlayerSessionId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-placed-player-session-schema.json
slug: gamelift-placed-player-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-placed-player-session-schema.json\",\n  \"title\": \"PlacedPlayerSession\",\n  \"description\": \"Information about a player session. This object contains only the player ID and player session ID. To retrieve full details on a player session, call <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribePlayerSessions.html\\\">DescribePlayerSessions</a> with the player session ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player that is associated with this player session.\"\n        }\n      ]\n    },\n    \"PlayerSessionId\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/PlayerSessionId\"\n        },\n        {\n          \"description\": \"A unique identifier for a player session.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-placed-player-session-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: PlacedPlayerSession
---
