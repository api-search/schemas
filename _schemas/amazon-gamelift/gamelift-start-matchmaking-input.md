---
description: StartMatchmakingInput schema from Amazon GameLift API
layout: schema
name: StartMatchmakingInput
properties_list:
- description: ''
  name: TicketId
  type: object
- description: ''
  name: ConfigurationName
  type: object
- description: ''
  name: Players
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-start-matchmaking-input-schema.json
slug: gamelift-start-matchmaking-input
source_filename: gamelift-start-matchmaking-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-matchmaking-input-schema.json\",\n  \"title\": \"StartMatchmakingInput\",\n  \"description\": \"StartMatchmakingInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for a matchmaking ticket. If no ticket ID is specified here, Amazon GameLift will generate one in the form of a UUID. Use this identifier to track the matchmaking ticket status and retrieve match results.\"\n        }\n      ]\n    },\n    \"ConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationName\"\n        },\n        {\n       \
  \   \"description\": \"Name of the matchmaking configuration to use for this request. Matchmaking configurations must exist in the same Region as this request. You can use either the configuration name or ARN value.\"\n        }\n      ]\n    },\n    \"Players\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerList\"\n        },\n        {\n          \"description\": \"<p>Information on each player to be matched. This information must include a player ID, and may contain player attributes and latency data to be used in the matchmaking process. After a successful match, <code>Player</code> objects contain the name of the team the player is assigned to.</p> <p>You can include up to 10 <code>Players</code> in a <code>StartMatchmaking</code> request.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationName\",\n    \"Players\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-start-matchmaking-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StartMatchmakingInput
---
