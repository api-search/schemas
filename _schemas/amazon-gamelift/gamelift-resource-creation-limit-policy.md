---
description: <p>A policy that puts limits on the number of game sessions that a player can create within a specified span of time. With this policy, you can control players' ability to consume available resources.</p> <p>The policy is evaluated when a player tries to create a new game session. On receiving a <code>CreateGameSession</code> request, Amazon GameLift checks that the player (identified by <code>CreatorId</code>) has created fewer than game session limit in the specified time period.</p>
layout: schema
name: ResourceCreationLimitPolicy
properties_list:
- description: ''
  name: NewGameSessionsPerCreator
  type: object
- description: ''
  name: PolicyPeriodInMinutes
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-resource-creation-limit-policy-schema.json
slug: gamelift-resource-creation-limit-policy
source_filename: gamelift-resource-creation-limit-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-resource-creation-limit-policy-schema.json\",\n  \"title\": \"ResourceCreationLimitPolicy\",\n  \"description\": \"<p>A policy that puts limits on the number of game sessions that a player can create within a specified span of time. With this policy, you can control players' ability to consume available resources.</p> <p>The policy is evaluated when a player tries to create a new game session. On receiving a <code>CreateGameSession</code> request, Amazon GameLift checks that the player (identified by <code>CreatorId</code>) has created fewer than game session limit in the specified time period.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NewGameSessionsPerCreator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n\
  \          \"description\": \"<p>A policy that puts limits on the number of game sessions that a player can create within a specified span of time. With this policy, you can control players' ability to consume available resources.</p> <p>The policy is evaluated when a player tries to create a new game session. On receiving a <code>CreateGameSession</code> request, Amazon GameLift checks that the player (identified by <code>CreatorId</code>) has created fewer than game session limit in the specified time period.</p>\"\n        }\n      ]\n    },\n    \"PolicyPeriodInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The time span used in evaluating the resource creation limit policy. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-resource-creation-limit-policy-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ResourceCreationLimitPolicy
---
