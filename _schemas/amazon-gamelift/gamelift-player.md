---
description: Represents a player in matchmaking. When starting a matchmaking request, a player has a player ID, attributes, and may have latency data. Team information is added after a match has been successfully completed.
layout: schema
name: Player
properties_list:
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: PlayerAttributes
  type: object
- description: ''
  name: Team
  type: object
- description: ''
  name: LatencyInMs
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-player-schema.json
slug: gamelift-player
source_filename: gamelift-player-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-player-schema.json\",\n  \"title\": \"Player\",\n  \"description\": \"Represents a player in matchmaking. When starting a matchmaking request, a player has a player ID, attributes, and may have latency data. Team information is added after a match has been successfully completed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player\"\n        }\n      ]\n    },\n    \"PlayerAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayerAttributeMap\"\n        },\n        {\n          \"description\": \"<p>A collection of key:value pairs containing player information\
  \ for use in matchmaking. Player attribute keys must match the <i>playerAttributes</i> used in a matchmaking rule set. Example: <code>\\\"PlayerAttributes\\\": {\\\"skill\\\": {\\\"N\\\": \\\"23\\\"}, \\\"gameMode\\\": {\\\"S\\\": \\\"deathmatch\\\"}}</code>.</p> <p>You can provide up to 10 <code>PlayerAttributes</code>.</p>\"\n        }\n      ]\n    },\n    \"Team\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Name of the team that the player is assigned to in a match. Team names are defined in a matchmaking rule set.\"\n        }\n      ]\n    },\n    \"LatencyInMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatencyMap\"\n        },\n        {\n          \"description\": \"<p>A set of values, expressed in milliseconds, that indicates the amount of latency that a player experiences when connected to @aws; Regions. If this property is present,\
  \ FlexMatch considers placing the match only in Regions for which latency is reported. </p> <p>If a matchmaker has a rule that evaluates player latency, players must report latency in order to be matched. If no latency is reported in this scenario, FlexMatch assumes that no Regions are available to the player and the ticket is not matchable. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-player-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: Player
---
