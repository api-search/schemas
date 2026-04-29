---
description: DescribeMatchmakingConfigurationsInput schema from Amazon GameLift API
layout: schema
name: DescribeMatchmakingConfigurationsInput
properties_list:
- description: ''
  name: Names
  type: object
- description: ''
  name: RuleSetName
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-matchmaking-configurations-input-schema.json
slug: gamelift-describe-matchmaking-configurations-input
source_filename: gamelift-describe-matchmaking-configurations-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-configurations-input-schema.json\",\n  \"title\": \"DescribeMatchmakingConfigurationsInput\",\n  \"description\": \"DescribeMatchmakingConfigurationsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationNameList\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking configuration(s) to retrieve. You can use either the configuration name or ARN value. To request all existing configurations, leave this parameter empty.\"\n        }\n      ]\n    },\n    \"RuleSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSetName\"\n        },\n    \
  \    {\n          \"description\": \"A unique identifier for the matchmaking rule set. You can use either the rule set name or ARN value. Use this parameter to retrieve all matchmaking configurations that use this rule set.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages. This parameter is limited to 10.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-configurations-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeMatchmakingConfigurationsInput
---
