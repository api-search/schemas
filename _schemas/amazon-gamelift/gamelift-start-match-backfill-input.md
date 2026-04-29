---
description: StartMatchBackfillInput schema from Amazon GameLift API
layout: schema
name: StartMatchBackfillInput
properties_list:
- description: ''
  name: TicketId
  type: object
- description: ''
  name: ConfigurationName
  type: object
- description: ''
  name: GameSessionArn
  type: object
- description: ''
  name: Players
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-start-match-backfill-input-schema.json
slug: gamelift-start-match-backfill-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-match-backfill-input-schema.json\",\n  \"title\": \"StartMatchBackfillInput\",\n  \"description\": \"StartMatchBackfillInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a matchmaking ticket. If no ticket ID is specified here, Amazon GameLift will generate one in the form of a UUID. Use this identifier to track the match backfill ticket status and retrieve match results.\"\n        }\n      ]\n    },\n    \"ConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationName\"\n        },\n        {\n\
  \          \"description\": \"Name of the matchmaker to use for this request. You can use either the configuration name or ARN value. The ARN of the matchmaker that was used with the original game session is listed in the <code>GameSession</code> object, <code>MatchmakerData</code> property.\"\n        }\n      ]\n    },\n    \"GameSessionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session. Use the game session ID. When using FlexMatch as a standalone matchmaking solution, this parameter is not needed. \"\n        }\n      ]\n    },\n    \"Players\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerList\"\n        },\n        {\n          \"description\": \"<p>Match information on all players that are currently assigned to the game session. This information is used by the matchmaker to find new players and add them\
  \ to the existing game.</p> <p>You can include up to 199 <code>Players</code> in a <code>StartMatchBackfill</code> request.</p> <ul> <li> <p>PlayerID, PlayerAttributes, Team -- This information is maintained in the <code>GameSession</code> object, <code>MatchmakerData</code> property, for all players who are currently assigned to the game session. The matchmaker data is in JSON syntax, formatted as a string. For more details, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-server.html#match-server-data\\\"> Match Data</a>. </p> <p>The backfill request must specify the team membership for every player. Do not specify team if you are not using backfill.</p> </li> <li> <p>LatencyInMs -- If the matchmaker uses player latency, include a latency value, in milliseconds, for the Region that the game session is currently in. Do not include latency values for any other Region.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationName\"\
  ,\n    \"Players\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-match-backfill-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StartMatchBackfillInput
---
