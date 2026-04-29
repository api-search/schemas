---
description: DescribeGameServerInstancesInput schema from Amazon GameLift API
layout: schema
name: DescribeGameServerInstancesInput
properties_list:
- description: ''
  name: GameServerGroupName
  type: object
- description: ''
  name: InstanceIds
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-game-server-instances-input-schema.json
slug: gamelift-describe-game-server-instances-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-instances-input-schema.json\",\n  \"title\": \"DescribeGameServerInstancesInput\",\n  \"description\": \"DescribeGameServerInstancesInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameServerGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupNameOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the game server group. Use either the name or ARN value.\"\n        }\n      ]\n    },\n    \"InstanceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerInstanceIds\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instance IDs that you want to retrieve status on. Amazon EC2 instance IDs use\
  \ a 17-character format, for example: <code>i-1234567890abcdef0</code>. To retrieve all instances in the game server group, leave this parameter empty. \"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameServerGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-game-server-instances-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeGameServerInstancesInput
---
