---
description: DescribeGameSessionDetailsInput schema from Amazon GameLift API
layout: schema
name: DescribeGameSessionDetailsInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: GameSessionId
  type: object
- description: ''
  name: AliasId
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: StatusFilter
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-session-details-input-schema.json
slug: gamelift-describe-game-session-details-input
source_filename: gamelift-describe-game-session-details-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-session-details-input-schema.json\",\n  \"title\": \"DescribeGameSessionDetailsInput\",\n  \"description\": \"DescribeGameSessionDetailsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to retrieve all game sessions active on the fleet. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"GameSessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the game session to retrieve. \"\n        }\n  \
  \    ]\n    },\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the alias associated with the fleet to retrieve all game sessions for. You can use either the alias ID or ARN value.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"A fleet location to get game session details for. You can specify a fleet's home Region or a remote location. Use the Amazon Web Services Region code format, such as <code>us-west-2</code>. \"\n        }\n      ]\n    },\n    \"StatusFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Game session status to filter results on. Possible game session statuses include <code>ACTIVE</code>,\
  \ <code>TERMINATED</code>, <code>ACTIVATING</code> and <code>TERMINATING</code> (the last two are transitory). \"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-session-details-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameSessionDetailsInput
---
