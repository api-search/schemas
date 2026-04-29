---
description: DescribeMatchmakingRuleSetsOutput schema from Amazon GameLift API
layout: schema
name: DescribeMatchmakingRuleSetsOutput
properties_list:
- description: ''
  name: RuleSets
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-matchmaking-rule-sets-output-schema.json
slug: gamelift-describe-matchmaking-rule-sets-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-rule-sets-output-schema.json\",\n  \"title\": \"DescribeMatchmakingRuleSetsOutput\",\n  \"description\": \"DescribeMatchmakingRuleSetsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSetList\"\n        },\n        {\n          \"description\": \"A collection of requested matchmaking rule set objects. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates where to resume retrieving results on the next call to this operation. If no token is returned, these results\
  \ represent the end of the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleSets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-rule-sets-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeMatchmakingRuleSetsOutput
---
