---
description: Regional latency information for a player, used when requesting a new game session. This value indicates the amount of time lag that exists when the player is connected to a fleet in the specified Region. The relative difference between a player's latency values for multiple Regions are used to determine which fleets are best suited to place a new game session for the player.
layout: schema
name: PlayerLatency
properties_list:
- description: ''
  name: PlayerId
  type: object
- description: ''
  name: RegionIdentifier
  type: object
- description: ''
  name: LatencyInMilliseconds
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-player-latency-schema.json
slug: gamelift-player-latency
source_filename: gamelift-player-latency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-player-latency-schema.json\",\n  \"title\": \"PlayerLatency\",\n  \"description\": \"Regional latency information for a player, used when requesting a new game session. This value indicates the amount of time lag that exists when the player is connected to a fleet in the specified Region. The relative difference between a player's latency values for multiple Regions are used to determine which fleets are best suited to place a new game session for the player. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlayerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a player associated with the latency data.\"\n        }\n      ]\n    },\n    \"RegionIdentifier\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Name of the Region that is associated with the latency value.\"\n        }\n      ]\n    },\n    \"LatencyInMilliseconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"Amount of time that represents the time lag experienced by the player when connected to the specified Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-player-latency-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: PlayerLatency
---
