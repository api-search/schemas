---
description: DescribeBuildOutput schema from Amazon GameLift API
layout: schema
name: DescribeBuildOutput
properties_list:
- description: ''
  name: Build
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-build-output-schema.json
slug: gamelift-describe-build-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-build-output-schema.json\",\n  \"title\": \"DescribeBuildOutput\",\n  \"description\": \"DescribeBuildOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Build\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Build\"\n        },\n        {\n          \"description\": \"Set of properties describing the requested build.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-build-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeBuildOutput
---
