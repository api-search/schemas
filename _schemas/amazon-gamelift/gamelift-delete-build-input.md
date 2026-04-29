---
description: DeleteBuildInput schema from Amazon GameLift API
layout: schema
name: DeleteBuildInput
properties_list:
- description: ''
  name: BuildId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-build-input-schema.json
slug: gamelift-delete-build-input
source_filename: gamelift-delete-build-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-build-input-schema.json\",\n  \"title\": \"DeleteBuildInput\",\n  \"description\": \"DeleteBuildInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BuildId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the build to delete. You can use either the build ID or ARN value. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BuildId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-build-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteBuildInput
---
