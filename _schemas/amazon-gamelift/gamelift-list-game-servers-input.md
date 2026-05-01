---
description: ListGameServersInput schema from Amazon GameLift API
layout: schema
name: ListGameServersInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: SortOrder
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-list-game-servers-input-schema.json
slug: gamelift-list-game-servers-input
source_filename: gamelift-list-game-servers-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-game-servers-input-schema.json\",\n  \"title\": \"ListGameServersInput\",\n  \"description\": \"ListGameServersInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"An identifier for the game server group to retrieve a list of game servers from. Use either the name or ARN value.\"\n        }\n      ]\n    },\n    \"SortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"Indicates how to sort the returned data based on game server registration timestamp. Use <code>ASCENDING</code>\
  \ to retrieve oldest game servers first, or use <code>DESCENDING</code> to retrieve newest game servers first. If this parameter is left empty, game servers are returned in no particular order.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-game-servers-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ListGameServersInput
---
