---
description: ValidateMatchmakingRuleSetOutput schema from Amazon GameLift API
layout: schema
name: ValidateMatchmakingRuleSetOutput
properties_list:
- description: ''
  name: Valid
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-validate-matchmaking-rule-set-output-schema.json
slug: gamelift-validate-matchmaking-rule-set-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-validate-matchmaking-rule-set-output-schema.json\",\n  \"title\": \"ValidateMatchmakingRuleSetOutput\",\n  \"description\": \"ValidateMatchmakingRuleSetOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Valid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanModel\"\n        },\n        {\n          \"description\": \"A response indicating whether the rule set is valid.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-validate-matchmaking-rule-set-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ValidateMatchmakingRuleSetOutput
---
