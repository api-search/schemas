---
description: CreateMatchmakingRuleSetOutput schema from Amazon GameLift API
layout: schema
name: CreateMatchmakingRuleSetOutput
properties_list:
- description: ''
  name: RuleSet
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-matchmaking-rule-set-output-schema.json
slug: gamelift-create-matchmaking-rule-set-output
source_filename: gamelift-create-matchmaking-rule-set-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-matchmaking-rule-set-output-schema.json\",\n  \"title\": \"CreateMatchmakingRuleSetOutput\",\n  \"description\": \"CreateMatchmakingRuleSetOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSet\"\n        },\n        {\n          \"description\": \"The newly created matchmaking rule set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleSet\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-matchmaking-rule-set-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateMatchmakingRuleSetOutput
---
