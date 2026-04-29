---
description: DescribeRuntimeConfigurationInput schema from Amazon GameLift API
layout: schema
name: DescribeRuntimeConfigurationInput
properties_list:
- description: ''
  name: FleetId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-runtime-configuration-input-schema.json
slug: gamelift-describe-runtime-configuration-input
source_filename: gamelift-describe-runtime-configuration-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-runtime-configuration-input-schema.json\",\n  \"title\": \"DescribeRuntimeConfigurationInput\",\n  \"description\": \"DescribeRuntimeConfigurationInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to get the runtime configuration for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-runtime-configuration-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeRuntimeConfigurationInput
---
