---
description: DescribeRuntimeConfigurationOutput schema from Amazon GameLift API
layout: schema
name: DescribeRuntimeConfigurationOutput
properties_list:
- description: ''
  name: RuntimeConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-runtime-configuration-output-schema.json
slug: gamelift-describe-runtime-configuration-output
source_filename: gamelift-describe-runtime-configuration-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-runtime-configuration-output-schema.json\",\n  \"title\": \"DescribeRuntimeConfigurationOutput\",\n  \"description\": \"DescribeRuntimeConfigurationOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuntimeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeConfiguration\"\n        },\n        {\n          \"description\": \"Instructions that describe how server processes should be launched and maintained on each instance in the fleet.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-runtime-configuration-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeRuntimeConfigurationOutput
---
