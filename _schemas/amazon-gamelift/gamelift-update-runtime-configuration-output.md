---
description: UpdateRuntimeConfigurationOutput schema from Amazon GameLift API
layout: schema
name: UpdateRuntimeConfigurationOutput
properties_list:
- description: ''
  name: RuntimeConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-runtime-configuration-output-schema.json
slug: gamelift-update-runtime-configuration-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-runtime-configuration-output-schema.json\",\n  \"title\": \"UpdateRuntimeConfigurationOutput\",\n  \"description\": \"UpdateRuntimeConfigurationOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuntimeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeConfiguration\"\n        },\n        {\n          \"description\": \"The runtime configuration currently in use by all instances in the fleet. If the update was successful, all property changes are shown. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-runtime-configuration-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateRuntimeConfigurationOutput
---
