---
description: DescribeMatchmakingConfigurationsOutput schema from Amazon GameLift API
layout: schema
name: DescribeMatchmakingConfigurationsOutput
properties_list:
- description: ''
  name: Configurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-matchmaking-configurations-output-schema.json
slug: gamelift-describe-matchmaking-configurations-output
source_filename: gamelift-describe-matchmaking-configurations-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-configurations-output-schema.json\",\n  \"title\": \"DescribeMatchmakingConfigurationsOutput\",\n  \"description\": \"DescribeMatchmakingConfigurationsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Configurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationList\"\n        },\n        {\n          \"description\": \"A collection of requested matchmaking configurations.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates where to resume retrieving results on the next call to this operation. If no token\
  \ is returned, these results represent the end of the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-configurations-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeMatchmakingConfigurationsOutput
---
