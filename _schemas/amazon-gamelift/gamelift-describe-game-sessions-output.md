---
description: DescribeGameSessionsOutput schema from Amazon GameLift API
layout: schema
name: DescribeGameSessionsOutput
properties_list:
- description: ''
  name: GameSessions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-sessions-output-schema.json
slug: gamelift-describe-game-sessions-output
source_filename: gamelift-describe-game-sessions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-sessions-output-schema.json\",\n  \"title\": \"DescribeGameSessionsOutput\",\n  \"description\": \"DescribeGameSessionsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameSessionList\"\n        },\n        {\n          \"description\": \"A collection of properties for each game session that matches the request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates where to resume retrieving results on the next call to this operation. If no token is returned, these results represent\
  \ the end of the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-sessions-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameSessionsOutput
---
