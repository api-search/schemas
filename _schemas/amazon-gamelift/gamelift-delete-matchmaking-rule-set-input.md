---
description: DeleteMatchmakingRuleSetInput schema from Amazon GameLift API
layout: schema
name: DeleteMatchmakingRuleSetInput
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-matchmaking-rule-set-input-schema.json
slug: gamelift-delete-matchmaking-rule-set-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-matchmaking-rule-set-input-schema.json\",\n  \"title\": \"DeleteMatchmakingRuleSetInput\",\n  \"description\": \"DeleteMatchmakingRuleSetInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSetName\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking rule set to be deleted. (Note: The rule set name is different from the optional \\\"name\\\" field in the rule set body.) You can use either the rule set name or ARN value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-matchmaking-rule-set-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteMatchmakingRuleSetInput
---
