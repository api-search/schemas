---
description: UpdateBuildOutput schema from Amazon GameLift API
layout: schema
name: UpdateBuildOutput
properties_list:
- description: ''
  name: Build
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-build-output-schema.json
slug: gamelift-update-build-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-build-output-schema.json\",\n  \"title\": \"UpdateBuildOutput\",\n  \"description\": \"UpdateBuildOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Build\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Build\"\n        },\n        {\n          \"description\": \"The updated build resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-build-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateBuildOutput
---
