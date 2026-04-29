---
description: DeleteMatchmakingConfigurationInput schema from Amazon GameLift API
layout: schema
name: DeleteMatchmakingConfigurationInput
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-matchmaking-configuration-input-schema.json
slug: gamelift-delete-matchmaking-configuration-input
source_filename: gamelift-delete-matchmaking-configuration-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-matchmaking-configuration-input-schema.json\",\n  \"title\": \"DeleteMatchmakingConfigurationInput\",\n  \"description\": \"DeleteMatchmakingConfigurationInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingConfigurationName\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking configuration. You can use either the configuration name or ARN value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-matchmaking-configuration-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteMatchmakingConfigurationInput
---
