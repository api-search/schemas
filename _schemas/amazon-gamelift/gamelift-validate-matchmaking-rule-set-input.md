---
description: ValidateMatchmakingRuleSetInput schema from Amazon GameLift API
layout: schema
name: ValidateMatchmakingRuleSetInput
properties_list:
- description: ''
  name: RuleSetBody
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-validate-matchmaking-rule-set-input-schema.json
slug: gamelift-validate-matchmaking-rule-set-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-validate-matchmaking-rule-set-input-schema.json\",\n  \"title\": \"ValidateMatchmakingRuleSetInput\",\n  \"description\": \"ValidateMatchmakingRuleSetInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleSetBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleSetBody\"\n        },\n        {\n          \"description\": \"A collection of matchmaking rules to validate, formatted as a JSON string.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleSetBody\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-validate-matchmaking-rule-set-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ValidateMatchmakingRuleSetInput
---
