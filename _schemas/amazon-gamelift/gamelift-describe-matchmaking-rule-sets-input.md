---
description: DescribeMatchmakingRuleSetsInput schema from Amazon GameLift API
layout: schema
name: DescribeMatchmakingRuleSetsInput
properties_list:
- description: ''
  name: Names
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-matchmaking-rule-sets-input-schema.json
slug: gamelift-describe-matchmaking-rule-sets-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-rule-sets-input-schema.json\",\n  \"title\": \"DescribeMatchmakingRuleSetsInput\",\n  \"description\": \"DescribeMatchmakingRuleSetsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSetNameList\"\n        },\n        {\n          \"description\": \"A list of one or more matchmaking rule set names to retrieve details for. (Note: The rule set name is different from the optional \\\"name\\\" field in the rule set body.) You can use either the rule set name or ARN value. \"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleSetLimit\"\n        },\n        {\n  \
  \        \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-rule-sets-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeMatchmakingRuleSetsInput
---
