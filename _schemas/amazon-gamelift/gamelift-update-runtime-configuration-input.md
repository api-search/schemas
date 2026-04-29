---
description: UpdateRuntimeConfigurationInput schema from Amazon GameLift API
layout: schema
name: UpdateRuntimeConfigurationInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: RuntimeConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-runtime-configuration-input-schema.json
slug: gamelift-update-runtime-configuration-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-runtime-configuration-input-schema.json\",\n  \"title\": \"UpdateRuntimeConfigurationInput\",\n  \"description\": \"UpdateRuntimeConfigurationInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to update runtime configuration for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"RuntimeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeConfiguration\"\n        },\n        {\n          \"description\": \"Instructions for launching server processes on each instance in the fleet.\
  \ Server processes run either a custom game build executable or a Realtime Servers script. The runtime configuration lists the types of server processes to run on an instance, how to launch them, and the number of processes to run concurrently.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"RuntimeConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-runtime-configuration-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateRuntimeConfigurationInput
---
