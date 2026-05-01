---
description: CreateMatchmakingConfigurationOutput schema from Amazon GameLift API
layout: schema
name: CreateMatchmakingConfigurationOutput
properties_list:
- description: ''
  name: Configuration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-matchmaking-configuration-output-schema.json
slug: gamelift-create-matchmaking-configuration-output
source_filename: gamelift-create-matchmaking-configuration-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-matchmaking-configuration-output-schema.json\",\n  \"title\": \"CreateMatchmakingConfigurationOutput\",\n  \"description\": \"CreateMatchmakingConfigurationOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfiguration\"\n        },\n        {\n          \"description\": \"Object that describes the newly created matchmaking configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-matchmaking-configuration-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateMatchmakingConfigurationOutput
---
