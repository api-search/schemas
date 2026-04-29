---
description: <p>Represents a new player session that is created as a result of a successful FlexMatch match. A successful match automatically creates new player sessions for every player ID in the original matchmaking request. </p> <p>When players connect to the match's game session, they must include both player ID and player session ID in order to claim their assigned player slot.</p>
layout: schema
name: MatchedPlayerSession
properties_list:
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: PlayerSessionId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-matched-player-session-schema.json
slug: gamelift-matched-player-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matched-player-session-schema.json\",\n  \"title\": \"MatchedPlayerSession\",\n  \"description\": \"<p>Represents a new player session that is created as a result of a successful FlexMatch match. A successful match automatically creates new player sessions for every player ID in the original matchmaking request. </p> <p>When players connect to the match's game session, they must include both player ID and player session ID in order to claim their assigned player slot.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player \"\n        }\n      ]\n    },\n    \"PlayerSessionId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/PlayerSessionId\"\n        },\n        {\n          \"description\": \"A unique identifier for a player session\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matched-player-session-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: MatchedPlayerSession
---
