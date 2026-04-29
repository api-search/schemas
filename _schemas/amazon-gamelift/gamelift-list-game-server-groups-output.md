---
description: ListGameServerGroupsOutput schema from Amazon GameLift API
layout: schema
name: ListGameServerGroupsOutput
properties_list:
- description: ''
  name: GameServerGroups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-list-game-server-groups-output-schema.json
slug: gamelift-list-game-server-groups-output
source_filename: gamelift-list-game-server-groups-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-game-server-groups-output-schema.json\",\n  \"title\": \"ListGameServerGroupsOutput\",\n  \"description\": \"ListGameServerGroupsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroups\"\n        },\n        {\n          \"description\": \"The game server groups' game server groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Specify the pagination token from a previous request to retrieve the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-game-server-groups-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ListGameServerGroupsOutput
---
